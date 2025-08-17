# hello-github
git status
#include <stdio.h>

#define MAX_STUDENTS 100

int main() {
    int n = 5; // Number of students
    float marks[] = {78, 65, 90, 55, 82};
    float sum = 0;
    float highest = marks[0];
    float lowest = marks[0];

    // Calculate sum, highest, and lowest marks
    for (int i = 0; i < n; i++) {
        sum += marks[i];
        if (marks[i] > highest) {
            highest = marks[i];
        }
        if (marks[i] < lowest) {
            lowest = marks[i];
        }
    }

    // Calculate average marks
    float average = sum / n;

    // Display results
    printf("Results:\n");
    printf("Average marks: %.2f\n", average);
    printf("Highest marks: %.2f\n", highest);
    printf("Lowest marks: %.2f\n", lowest);

    // Display student-wise marks
    printf("\nStudent-wise marks:\n");
    for (int i = 0; i < n; i++) {
        printf("Student %d: %.2f\n", i + 1, marks[i]);
    }

    return 0;
}
