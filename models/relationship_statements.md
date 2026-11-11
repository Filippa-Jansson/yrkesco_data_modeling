# Relationship statements

## Program och Klass

Ett program kan ha flera klasser, men varje klass tillhör ett program.
Detta följer kravspecifikationen där ett program kan genomföras flera gånger, vilket innebär att samma program kan ha flera klasser över tid.

## Program och Kurs

Ett program innehåller flera kurser, men varje kurs tillhör ett program.
Detta gör det möjligt att definiera vilka kurser som ingår i ett visst utbildningsprogram.

## Utbildningsledare och Klass

En utbildningsledare ansvarar för flera klasser, men varje klass har en utbildningsledare.
Detta motsvarar kravet att en utbildningsledare har ansvar för flera klasser inom organisationen.

## Klass och Student

En klass kan innehålla flera studenter, men varje student tillhör en klass.
Detta gör det möjligt att koppla studenter till rätt programomgång och att hålla reda på vilka studenter som studerar tillsammans.

## Student och Studentuppgifter

Varje student har en uppsättning studentuppgifter, och varje post i studentuppgifter tillhör en student.
Denna uppdelning används för att lagra känsliga personuppgifter separat från övrig studentinformation, vilket gör det enklare att kontrollera åtkomst till dessa uppgifter.

## Utbildare och Kurs

En utbildare kan undervisa flera kurser, men varje kurs har en ansvarig utbildare.
Detta gör det möjligt att se vilken utbildare som ansvarar för en specifik kurs inom ett program.

## Utbildare och Klass

En utbildare kan vara kopplad till flera klasser och en klass kan ha flera utbildare.
Denna relation hanteras i databasen genom kopplingstabellen Utbildare_klass eftersom det är en many-to-many-relation.

## Utbildare och Konsult

En utbildare kan även vara konsult, men behöver inte vara det. Varje post i tabellen "Konsult" representerar en utbildare som arbetar som konsult.

## Konsult och Konsultföretag

Ett konsultföretag kan ha flera konsulter, men varje konsult är kopplad till ett specifikt konsultföretag.
Detta gör det möjligt att lagra information om konsultföretag och vilka konsulter som arbetar för dem.

## Konsult och Konsultavgift

Varje konsult har en konsultavgift som beskriver konsultens timarvode.
Denna information lagras i en separat tabell för att separera ekonomisk information från övrig konsultdata och hålla det privat.
