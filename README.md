# Medical-Diagnosis-Grading-and-Treatment-System-According-to-Patient-Severity-
This projects step up by using the concepts of C such loops, conditional statement, logical operators to distinguish patients in grades (A to D) and provides proper medical staff and resources to the cure the patient
#include <stdio.h>

void main() {
    char grade;

    printf("Enter patient severity grades (A, B, C, D).\n");
    printf("Grades explanation : \n A : Near death condition or critically injured \n ");
    printf("B : Multiple Fracture or Deep cuts  \n ");
    printf("C : Minor Injury or High Fever  \n ");
    printf("D : Minor Cold or Cough \n ");
    printf("\n");

    printf("Enter grade: "); 
    scanf("%c", &grade);

    
    if (grade == 'A'|| grade == 'a') {
        printf("Severity: Critical\nResources allocated:\n- ICU Bed\n- Ventilator\nStaff assigned:\n- Intensivist\n- Senior Nurse\n");
    } 
    else if (grade == 'B'|| grade == 'b') {
        printf("Severity: High\nResources allocated:\n- High Dependency Unit\nStaff assigned:\n- Specialist Physician\n- Nurse\n");
    } 
    else if (grade == 'C' || grade =='c') {
        printf("Severity: Moderate\nResources allocated:\n- General Ward\nStaff assigned:\n- General Physician\n- Junior Nurse\n");
    } 
    else if (grade == 'D' || grade == 'd') {
        printf("Severity: Low\nResources allocated:\n- Outpatient Care\nStaff assigned:\n- General Practitioner\n");
    } 
    else {
        printf("Invalid grade. Please enter A, B, C, D \n");
    }

    }
