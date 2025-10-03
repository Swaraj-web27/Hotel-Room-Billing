Name- Swaraj Wanjale
Department- Computer Engineering
Roll no.- 122
Division- CE2

1. Introduction
A hotel room booking system is a software application designed to facilitate the process of reserving rooms at a hotel. It allows customers to book rooms based on their preferences, such as room type and stay duration, while also managing pricing. This system improves operational efficiency for hotels and enhances customer experience by providing a quick and easy way to book rooms.

2. Ideate 
Accept customer details : name and phone number. Allow selection of room type like Standard, Deluxe or Suite. Provide the respective rate of the room. Take the number of nights the person would like to stay. Calculate total bill. Calculate the total price based on the room rate and nights.

3. Analysis
The system uses characters that store textual information like customer name, phone number, and room type, while integers track numeric values like the number of nights, total bill. The program ensures that only valid room types (Standard, Deluxe , Suite) are accepted. Prices are fixed and multiplied by the number of nights for total cost calculation.






4. Built
#include<stdio.h>
void main(){
    char name[50],type; 
    int cust_no, no_of_days,roomtype,rate;
    printf("Enter Customer name:");
    scanf("%s",name);
    printf("Enter Phone number:");
    scanf("%s",&cust_no);
    printf("\n\nPlease select which room would you like:\n1.Standard (1000 Rs per night)\n2.Deluxe (2000 Rs per night)\n3.Suite (3000 Rs per night)\nEnter Your choice:");
    scanf("%d",&roomtype);
    if (roomtype==1){
        printf("\nStandard room has been booked!\n");
        rate=1000;
        printf("Rate of the room booked=%dRs\n",rate);
        printf("Enter Number of days you would like to stay:");
        scanf("%d",&no_of_days);
        printf("Total bill=%d Rs",rate*no_of_days);
        printf("\n\nCustomer Name:%s\n",name);
        printf("Phone Number:%d\n",cust_no);
        printf("Room Booked = Standard\n");
        printf("Number of days you are staying:%d",no_of_days);
        printf("\nTotal Bill = %dRs",rate*no_of_days);
    }
    else if(roomtype==2){
        printf("\nDeluxe room has been booked!\n");
        rate=2000;
        scanf("Deluxe",&type);
        printf("Rate of the room booked=%dRs\n",rate);
        printf("Enter Number of days you would like to stay:");
        scanf("%d",&no_of_days);
        printf("Total bill=%d Rs",rate*no_of_days);
        printf("\n\nCustomer Name:%s\n",name);
        printf("Phone Number:%d\n",cust_no);
        printf("Room Booked = Deluxe\n");
        printf("Number of days you are staying:%d",no_of_days);
        printf("\nTotal Bill = %dRs",rate*no_of_days);
    }
    else if(roomtype==3){
        printf("\nSuite has been booked\n");
        rate=3000;
        scanf("Suite",&type);;
        printf("Rate of the room booked=%dRs\n",rate);
        printf("Enter Number of days you would like to stay:");
        scanf("%d",&no_of_days);
        printf("Total bill=%d Rs",rate*no_of_days);
        printf("\n\nCustomer Name:%s\n",name);
        printf("Phone Number:%d\n",cust_no);
        printf("Room Booked = Suite\n");
        printf("Number of days you are staying:%d",no_of_days);
        printf("\nTotal Bill = %dRs",rate*no_of_days);
    }
    else{
        printf("Please select a valid value");
    }
}

5. Testing

Output 1
Enter Customer name:ABC
Enter Phone number:1234567890


Please select which room would you like:
1.Standard (1000 Rs per night)
2.Deluxe (2000 Rs per night)
3.Suite (3000 Rs per night)
Enter Your choice:1

Standard room has been booked!
Rate of the room booked=1000Rs
Enter Number of days you would like to stay:4
Total bill=4000 Rs

Customer Name:ABC
Phone Number:1234567890
Room Booked = Standard
Number of days you are staying:4
Total Bill = 4000Rs

Output 2 
Enter Customer name:XYZ
Enter Phone number:1234567890


Please select which room would you like:
1.Standard (1000 Rs per night)
2.Deluxe (2000 Rs per night)
3.Suite (3000 Rs per night)
Enter Your choice:2

Deluxe room has been booked!
Rate of the room booked=2000Rs
Enter Number of days you would like to stay:55
Total bill=110000 Rs

Customer Name:XYZ
Phone Number:1234567890
Room Booked = Deluxe
Number of days you are staying:55
Total Bill = 110000Rs

6. Implementation 
The project is published on google for easy access to the code.
https://github.com/Swaraj-web27/Hotel-Room-Billing/tree/main

7. Conclusion
The hotel room billing system developed successfully automates the process of booking rooms and calculating the total bill based on customer preferences. By accepting essential customer details and allowing selection among different room types with fixed rates, the system ensures accurate and efficient billing.
