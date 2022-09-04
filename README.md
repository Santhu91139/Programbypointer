
// This is a C program to add two distances in feet and inches by using pointers

#include <stdio.h>
struct Distance
{
   int feet;
   int inch;
};
void main()
{
struct Distance d1,d2,result;
   printf("Enter 1st distance\n");
   printf("Enter feet:\n");
   scanf("%d", &d1.feet);
   printf("Enter inch:\n");
   scanf("%d", &d1.inch);
   printf("Enter 2nd distance\n");
   printf("Enter feet:\n");
   scanf("%d", &d2.feet);
   printf("Enter inch:\n");
   scanf("%d", &d2.inch);
   result.feet = d1.feet + d2.feet;
   result.inch = d1.inch + d2.inch;
   while (result.inch >= 12)
{
      result.inch = result.inch - 12;
      ++result.feet;
   printf("Sum of distances = %d.%d\n", result.feet, result.inch);
}
}
