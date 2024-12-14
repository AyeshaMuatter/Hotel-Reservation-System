# Hotel-Reservation-System 
#include <iostream>
using namespace std;
/ Room types and prices
int singleroomprice = 4000;
int doubleroomprice = 8000;
int suiteroomprice = 16000;

// Maximum room counts
int maxsinglerooms = 10;
int maxdoublerooms = 5;
int maxsuiterooms = 2;

// Room availability
int availableRooms[3] = {maxsinglerooms, maxdoublerooms, maxsuiterooms};

// Booking information
string customers[100];         // Store customer names
int bookingHistory[100][3];    // Customer ID, Room Type, Nights
int totalCustomers = 0;        // Track number of customers

void checkAvailability() {
    cout << "\nRoom Availability:\n";
    cout << "1. Single Rooms: " << availableRooms[0] << " available\n";
    cout << "2. Double Rooms: " << availableRooms[1] << " available\n";
    cout << "3. Suite Rooms: " << availableRooms[2] << " available\n";
}
