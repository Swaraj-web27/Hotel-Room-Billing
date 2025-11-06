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
