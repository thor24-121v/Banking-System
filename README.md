# Banking-System
This System or project is for those who works in banks
if you want to get other atm system which scans from this file than check atm banking system


#include <stdio.h>
#include <time.h>

struct customer
{

    char name[20];
    int account;
    int balance;
    int code;
    int amount;

} cus1, cus2, cus3, cus4, detail;

int main()
{
    FILE *ptr;
    ptr = fopen("bank_file.txt", "a");

    int nc, i, amnc, choose, total;

    printf("Enter Number of Customers : ");
    scanf("%d", &nc);

    for (i = 0; i != nc; i++)
    {

        printf("Enter Customer Name : ");
        scanf("%s", cus1.name);

fprintf(ptr, "%s\n", cus1.name);

        printf("Enter Account Number : ");
        scanf("%d", &cus1.account);

fprintf(ptr, "%d\n", cus1.account);

        printf("Enter Balance in Account : ");
        scanf("%d", &cus1.balance);

fprintf(ptr, "%d\n", cus1.balance);

        printf("---------------------------------------------------\n");

        printf("Enter Customer Name : ");
        scanf("%s", cus3.name);

 fprintf(ptr, "%s\n", cus3.name);


        printf("Enter Account Number : ");
        scanf("%d", &cus3.account);

fprintf(ptr, "%d\n", cus3.account);


        printf("Enter Balance in Account : ");
        scanf("%d", &cus3.balance);

fprintf(ptr, "%d\n", cus3.balance);

         printf("---------------------------------------------------\n");

        printf("Enter Customer Name : ");
        scanf("%s", cus4.name);

fprintf(ptr, "%s\n", cus4.name);

        printf("Enter Account Number : ");
        scanf("%d", &cus4.account);

fprintf(ptr, "%d\n", cus4.account);

        printf("Enter Balance in Account : ");
        scanf("%d", &cus4.balance);

fprintf(ptr, "%d\n", cus4.balance);

        if (nc > 200)
        {
            printf("Maximum Number Of Customer is 200\n");
            break;
        }
    }
    fclose(ptr);

   
}
