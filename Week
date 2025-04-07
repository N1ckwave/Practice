#include <stdio.h>
#include <stdlib.h>

#ifdef _WIN32
    #define CLEAR_SCREEN "cls"  // Windows command for clearing screen
#else
    #define CLEAR_SCREEN "clear"  // Linux/macOS command for clearing screen
#endif

void drawTriangles(int size) {
    // Right-angled triangle
    for (int i = 1; i <= size; i++) {
        for (int j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }

    printf("\n");

    // Inverted right-angled triangle
    for (int i = size; i >= 1; i--) {
        for (int j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }
}

int main() {
    char name[50];
    char date[11]; // Format: yyyy-mm-dd

    // Get user input
    printf("Enter your name: ");
    scanf("%49s", name);
    printf("Enter today's date (yyyy-mm-dd): ");
    scanf("%10s", date);

    // Display welcome message
    printf("\nWelcome, %s! Today is %s.\n", name, date);

    // Pause for 3 seconds before clearing the screen
    printf("\nPreparing splash screen...\n");
    system("sleep 3"); // Works on Unix/macOS
    system(CLEAR_SCREEN); // Clears the screen

    // Display splash screen with triangles
    printf("\n========================================\n");
    printf("    WELCOME TO THE MAGRATHEA PROJECT   \n");
    printf("========================================\n\n");

    drawTriangles(5); // Print triangles with size 5

    printf("\nSystem Ready!\n");
    
    return 0;
}
