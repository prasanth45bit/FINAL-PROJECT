#include<stdio.h>
#include<string.h>
struct bank
{
    int pass;
    char user[50];
    int balance;
    char name[50];
    int phone;
    char mail[50];
    char loantype[50];
    int loan,lc;
    int accno;
} l;
void loan()
{
    printf("\n-\t-\t-\t-\tLOAN APPLY\t-\t-\t-\t-\n");
    printf("\n1.HOME LOAN       ");
    printf("\n2.CAR  LOAN       ");
    printf("\n3.EDUCATIONAL LOAN");
    printf("\n4.AGRI LOAN       ");
    printf("\nEnter your choise:");
    scanf("%d",&l.lc);
    if(l.lc==1)
    {
        int c;
        strcpy(l.loantype,"HOMELOAN");
        printf("\n-\t-\t-\t-\t%s\t-\t-\t-\t-\n",l.loantype);
        printf("\nLoan Amount details");
        printf("\n1.500000\n2.1000000");
        printf("\nEnter the choise:");
        scanf("%d",&c);
        if(c>0 &&c<3)
        {
            if(c==1)
            {
                l.loan=500000;
            }
            if(c==2)
            {
                l.loan=1000000;
            }
            printf("Loan amount succsefully sanctioned");
        }
    }
    if(l.lc==2)
    {
        int c;
        strcpy(l.loantype,"CARLOAN");
        printf("\n-\t-\t-\t-\t%s\t-\t-\t-\t-\n",l.loantype);
        printf("\nLoan Amount details");
        printf("\n1.400000\n2.800000");
        printf("\nEnter the choise:");
        scanf("%d",&c);
        if(c>0 &&c<3)
        {
            if(c==1)
            {
                l.loan=400000;
            }
            if(c==2)
            {
                l.loan=800000;
            }
            printf("Loan amount succsefully sanctioned");
        }
    }
    if(l.lc==3)
    {
        int c;
        strcpy(l.loantype,"EDUCATIONALLOAN");
        printf("\n-\t-\t-\t-\t%s\t-\t-\t-\t-\n",l.loantype);
        printf("\nLoan Amount details");
        printf("\n1.100000 per year\n2.200000 per year");
        printf("\nEnter the choise:");
        scanf("%d",&c);
        if(c>0 &&c<3)
        {
            if(c==1)
            {
                l.loan=100000;
            }
            if(c==2)
            {
                l.loan=200000;
            }
            printf("\nLoan amount succsefully sanctioned");
        }
    }
    if(l.lc==4)
    {
        int c;
        strcpy(l.loantype,"AGRILOAN");
        printf("\n-\t-\t-\t-\t%s\t-\t-\t-\t-\n",l.loantype);
        printf("\nLoan Amount details");
        printf("1.100000 per acre\n2.200000");
        printf("\nEnter the choise:");
        scanf("%d",&c);
        if(c>0 &&c<3)
        {
            if(c==1)
            {
                l.loan=100000;
            }
            if(c==2)
            {
                l.loan=200000;
            }
            printf("Loan amount succsefully sanctioned");
        }
        else
        {
            printf("\nInvalid Option");
        }
    }
}
void menu()
{
    int a=0;
    do
    {
        int mc;
        printf("\n-\t-\t-\t-\tMENU\t-\t-\t-\t-\n");
        printf("\n1.PROFILE\n");
        printf("2.DEPOSIT AMOUNT\n");
        printf("3.WITHDRAW AMOUNT\n");
        printf("4.CHECK BALANCE\n");
        printf("5.APPLY LOAN\n");
        printf("6.YOUR LOAN DETAILS\n");
        printf("7.EXIT");
        printf("\n-\t-\t-\t-\t-\n");
        printf("\nEnter Your choice:");
        scanf("%d",&mc);
        if(mc==1)
        {
            int change;
            int newpass;
            int passn;
            printf("\nYour name:%s", l.name);
            printf("\nYour phone number:%d", l.phone);
            printf("\nYour mail id:%s", l.mail);
            printf("\nYour account number:%d",l.accno);
            printf("\nChange password \n 1.Yes \t 2.No:");
            scanf("%d", &change);
            if(change==1)
            {
                printf("\nEnter your password:");
                scanf("%d",&passn);
                if(l.pass==passn)
                {
                    printf("\nEnter your new password:");
                    scanf("%d",&newpass);
                    l.pass=newpass;
                    printf("\nPassword Changed Successfully!");
                }
                else
                {
                    printf("Password Wrong");
                }
            }
        }
        if(mc == 2)
        {
            int depo;
            printf("\n-\t-\t-\t-\tDEPOSIT\t-\t-\t-\t-\n");
            printf("Enter the amount:");
            scanf("%d",&depo);
            l.balance+=depo;
            printf("\nAmount deposited successfully");
        }
        if(mc==3)
        {
            int with;
            int passl;
            printf("\n-\t-\t-\t-\tWITHDRAW\t-\t-\t-\t-\n");
            printf("Enter the password:");
            scanf("%d",&passl);
            if(l.pass==passl)
            {
                printf("Enter the amount:");
                scanf("%d",&with);
                if(l.balance>=with)
                {
                    l.balance-=with;
                    printf("\nAmount withdrawn successfully");
                }
                else
                {
                    printf("Insufficient balance");
                }
            }
            else
            {
                printf("\nPassword incorrect");
            }
        }
        if(mc == 4)
        {
            int passl;
            printf("\n-\t-\t-\t-\tBALANCE check\t-\t-\t-\t-\n");
            printf("Enter the password:");
            scanf("%d", &passl);
            if(l.pass==passl)
            {
                printf("\nYOUR BANK BALANCE IS %d",l.balance);
            }
            else
            {
                printf("\nPassword incorrect");
            }
        }
        if(mc==5)
        {
            loan();
        }
        if(mc==6)
        {
            int lpay,payamount;
            printf("\nYour loan amount is:%d",l.loan);
            printf("\nPay loan\n 1.Yes 2.No:");
            scanf("%d",&lpay);
            if(lpay==1)
            {
                printf("\nEnter instalment amount:");
                scanf("%d",&payamount);
                if(l.loan=payamount)
                {
                    printf("\nLoan instalment completed");
                    printf("\nPayment sucessfully");
                }
                else if(l.loan>payamount)
                {
                    printf("\nPayment succsefully");
                    printf("\nBalance loan amount:%d",l.loan-payamount);
                }
            }
        }
        if(mc==7)
        {
            printf("Exiting...\nThank you so much");
            a=10;
            break;
        }
        else
        {
            printf("Invalid Choise:");
        }
    } while(a==0);
}
void create()
{
    int i=0;
    int passc;
    l.loan=0;
    for(i=0;i<3;)
    {
        printf("\n-\t-\t-\t-\tSIGN UP\t-\t-\t-\t-\n");
        printf("\nCreate Your Username:");
        scanf("%s",l.user);
        printf("\nCreate Your Password:");
        scanf("%d",&l.pass);
        printf("\nConfirm Your password:");
        scanf("%d",&passc);
        l.accno=1001;
        if(l.pass==passc)
        {
            printf("\nAccount Created Successfully\n");
            printf("\nEnter your name:");
            scanf("%s",l.name);
            printf("\nEnter your phone number:");
            scanf("%d",&l.phone);
            printf("\nEnter your Email id:");
            scanf("%s",l.mail);
            printf("Enter the initial deposit amount:");
            scanf("%d",&l.balance);
            menu();
            break;
        }
        else
        {
            printf("Password miss match\n");
            i++;
        }
    }
    if(i >= 3)
    {
        printf("\nMaximum login reach\n");
    }
}

void check(char user1[50],int pass1)
{
    int i;
    for(i=0;i<3;)
    {
        if((!strcmp(user1,l.user) && pass1==l.pass) || (!strcmp(l.user,"prasanth") && pass1==1234))
        {
            printf("\nLogin Successfully\n");
            if(!strcmp(user1,"prasanth"))
            {
                strcpy(l.name,"HITMAN");
                l.phone=1234567890;
                strcpy(l.mail,"prasa12334");
                l.balance=20000;
                l.loan=15000;
                l.accno=1000;
                menu();
            }
            break;
        }
        else
        {
            printf("Username or Password is Invalid\n");
            i++;
        }
    }
    if(i >= 3)
    {
        printf("\nMaximum login reached\n");
    }
}

int login()
{
    printf("\n-\t-\t-\t-\tLOGIN\t-\t-\t-\t-\n");
    int pass1=1234;
    char user1[50]="prasanth";
    printf("\nEnter Your Username:");
    scanf("%s",l.user);
    printf("\nEnter Your Password:");
    scanf("%d",&l.pass);
    check(l.user,l.pass);
}
int main()
{
    int choice;
    printf("\t\t\t\t$$$$$$$$$$$$$$$$$$$$$$\n");
    printf("\t\t\t\tWELCOME OUR BANK USERS!\n");
    printf("\t\t\t\t$$$$$$$$$$$$$$$$$$$$$$\n");
    printf("1. LOGIN\n2. SIGN UP\n");
    printf("\nEnter Your Choice:");
    scanf("%d", &choice);
    switch(choice)
    {
        case 1:
            login();
            break;
        case 2:
            create();
            break;
        default:
            printf("Choice Invalid. Try again later.");
            break;
    }
    return 0;
}

