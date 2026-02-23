# Online-movie-ticket-booking-using-c
#include <stdio.h>
#include <stdlib.h>

int main() {
    int choice, tickets;
    int day,month,year;
   float price, total;

    printf("\n===== ONLINE MOVIE TICKET BOOKING =====\n");
    printf("1. Leo - Rs.150\n");
    printf("2. Jawan - Rs.180\n");
    printf("3. Vikram - Rs.200\n");
    printf("4. Avengers - Rs.250\n");
    printf("5. Exit\n");

    printf("\nSelect a movie (1-5): ");
    scanf("%d", &choice);

    switch(choice) {
        case 1:
            price = 150;
            printf("You selected Leo\n");
            break;
        case 2:
            price = 180;
            printf("You selected Jawan\n");
            break;
        case 3:
            price = 200;
            printf("You selected Vikram\n");
            break;
        case 4:
            price = 250;
            printf("You selected Avengers\n");
            break;
        case 5:
            printf("Thank you! Visit Again.\n");
            exit(0);
        default:
            printf("Invalid Choice!\n");
            return 0;
    }
    printf("\nEnter Show Date (DD MM YYYY): ");
    scanf("%d %d %d", &day, &month, &year);
       printf("Enter number of tickets:");
    scanf("%d", &tickets);
    
     total = price * tickets;

    printf("\n===== BOOKING CONFIRMATION =====\n");
    printf("Number of Tickets: %d\n", tickets);
    printf("Total Amount: Rs. %.2f\n", total);
    printf("Booking Successful!\n");
    return 0;
    }
