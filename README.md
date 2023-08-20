#*******Skillrack_Dialy_Challenge3*******
#Program to convert python program to c program
  #include <stdio.h>
  #include <stdlib.h>
  #include <string.h>

  int main() {
      int num[1001];
      char str[1001];
    
      fgets(str, sizeof(str), stdin);
      char *token = strtok(str, " ");
      int count = 0;
    
      while (token != NULL) {
          num[count] = abs(atoi(token)) % 2;
          count++;
          token = strtok(NULL, " ");
      }
    
      int sum = 0;
      for (int i = 0; i < count; i++) {
          sum += num[i];
      }
    
      printf("%d", sum);
    
      return 0;
  }
#Skillrack_Dialy_Challenge3
