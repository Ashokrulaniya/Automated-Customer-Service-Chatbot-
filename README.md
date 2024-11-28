# Automated-Customer-Service-Chatbot-
This a customer service chatbot end to end project

like this code ! :)

#include <stdio.h> 
// Function to display the main menu and return the user's choice 
int mainMenu() { 
int choice; 
printf("\nWelcome to Customer Support Chatbot!\n"); 
printf("Please choose a category:\n"); 
printf("1. Product Information\n"); 
printf("2. Billing and Payment\n"); 
printf("3. Technical Support\n"); 
printf("4. Talk to a Human Agent\n"); 
printf("5. Exit\n"); 
printf("Enter your choice: "); 
scanf("%d", &choice); 
return choice; 
} 
// Function to handle Product Information queries 
void productInfo() { 
int choice; 
printf("\nProduct Information:\n"); 
printf("1. Pricing\n"); 
printf("2. Availability\n"); 
printf("3. Specifications\n"); 
printf("4. Back to Main Menu\n"); 
printf("Enter your choice: "); 
scanf("%d", &choice); 
switch (choice) { 
case 1: 
printf("Our products are competitively priced to offer the best value for your money.\n"); 
            break; 
        case 2: 
            printf("The product is currently available in stock.\n"); 
            break; 
        case 3: 
            printf("The product has high specifications, including 16GB RAM and 1TB SSD.\n"); 
            break; 
        case 4: 
            break; 
        default: 
            printf("Invalid choice. Returning to Main Menu.\n"); 
            break; 
    } 
} 
 
// Function to handle Billing and Payment queries 
void billingPayment() { 
    int choice; 
    printf("\nBilling and Payment:\n"); 
    printf("1. Check Invoice\n"); 
    printf("2. Payment Options\n"); 
    printf("3. Refund Policy\n"); 
    printf("4. Back to Main Menu\n"); 
    printf("Enter your choice: "); 
    scanf("%d", &choice); 
 
    switch (choice) { 
        case 1: 
            printf("You can check your invoice by logging into your account on our website.\n"); 
            break; 
        case 2: 
            printf("We accept all major credit cards, debit cards, and PayPal.\n"); 
            break; 
        case 3: 
            printf("Our refund policy allows returns within 30 days of purchase.\n"); 
            break; 
        case 4: 
            break; 
        default: 
            printf("Invalid choice. Returning to Main Menu.\n"); 
            break; 
    } 
} 
 
// Function to handle Technical Support queries 
void technicalSupport() { 
    int choice; 
    printf("\nTechnical Support:\n"); 
    printf("1. Troubleshooting\n"); 
    printf("2. Warranty Information\n"); 
    printf("3. Software Updates\n"); 
    printf("4. Back to Main Menu\n"); 
    printf("Enter your choice: "); 
    scanf("%d", &choice); 
 
    switch (choice) { 
        case 1: 
            printf("Please restart your device and try again. If the problem persists, contact our support 
team.\n"); 
            break; 
        case 2: 
            printf("Your product comes with a 1-year warranty from the date of purchase.\n"); 
            break; 
        case 3: 
            printf("You can download the latest software updates from our official website.\n"); 
            break; 
        case 4: 
            break; 
        default: 
            printf("Invalid choice. Returning to Main Menu.\n"); 
            break; 
    } 
} 
 
// Function to simulate escalation to a human agent 
void talkToHumanAgent() { 
    printf("\nConnecting you to a human agent... Please wait.\n"); 
} 
 
int main() { 
    int choice; 
 
    while (1) { 
        choice = mainMenu(); 
 
        switch (choice) { 
            case 1: 
                productInfo(); 
                break; 
            case 2: 
                billingPayment(); 
                break; 
            case 3: 
                technicalSupport(); 
                break; 
            case 4: 
                talkToHumanAgent(); 
                break; 
            case 5: 
                printf("Thank you for chatting with us. Goodbye!\n"); 
                return 0; 
            default: 
                printf("Invalid choice. Please try again\n);
          } 
    } 
 
    return 0; 
} 
