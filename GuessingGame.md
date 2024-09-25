```mermaid
flowchart TD
Start([Start]) --> B[Integer SecretNumber] --> C[Integer UserGuess] --> D[SecretNumber = n-1 = Random 21] --> E[/Output "Please enter a number between 0 and 20"/]
--> F[/Input UserGuess/]    
--> G{{UserGues <> SecretNumber}}
G -- False --> H{UserGuess < SecretNumber} --> I[/Output Higher/] --> F
G -- False --> J{UserGuess > Secret Number} --> K[/Output Lower/] --> F
G --> True --> L[/Output "Congrats! That's Correct. Thank you for playing"/]
--> End([End])
