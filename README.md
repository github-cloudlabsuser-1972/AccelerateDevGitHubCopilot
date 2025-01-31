Collecting workspace information

# Library App

## Description
Library App is a console-based application for managing a library system. It allows users to search for patrons, renew memberships, return loaned books, and extend book loans. The application uses JSON files to store data about authors, books, book items, patrons, and loans.

## Project Structure
- 

src


  - 

Library.ApplicationCore/


    - 

Entities/


      - 

Author.cs


      - 

Book.cs


      - 

BookItem.cs


      - 

Loan.cs


      - 

Patron.cs


    - 

Enums/


      - 

EnumHelper.cs


      - 

LoanExtensionStatus.cs


      - 

LoanReturnStatus.cs


      - 

MembershipRenewalStatus.cs


    - `Interfaces/`
      - 

ILoanRepository.cs


      - 

ILoanService.cs


      - 

IPatronRepository.cs


      - 

IPatronService.cs


    - `Services/`
      - 

LoanService.cs


      - 

PatronService.cs


    - 

Library.ApplicationCore.csproj


  - 

Library.Console/


    - 

appSettings.json


    - 

CommonActions.cs


    - 

ConsoleApp.cs


    - 

ConsoleState.cs


    - 

Json/


      - 

Authors.json


      - 

Books.json


      - 

BookItems.json


      - 

Loans.json


      - 

Patrons.json


    - 

Library.Console.csproj


    - 

Program.cs


  - 

Library.Infrastructure/


    - 

Data/


      - 

JsonData.cs


      - 

JsonLoanRepository.cs


      - 

JsonPatronRepository.cs


    - 

Library.Infrastructure.csproj


- 

tests


  - 

UnitTests/


    - 

ApplicationCore/


      - 

LoanService/


        - 

ExtendLoan.cs


        - 

ReturnLoan.cs


      - 

PatronService/


        - 

RenewMembership.cs


    - 

LoanFactory.cs


    - 

PatronFactory.cs


    - 

UnitTests.csproj



## Key Classes and Interfaces
- **Entities**
  - 

Author

: Represents an author.
  - 

Book

: Represents a book.
  - 

BookItem

: Represents a physical copy of a book.
  - 

Loan

: Represents a loan of a book item to a patron.
  - 

Patron

: Represents a library patron.
- **Enums**
  - 

EnumHelper

: Provides helper methods for enums.
  - 

LoanExtensionStatus

: Enum for loan extension statuses.
  - 

LoanReturnStatus

: Enum for loan return statuses.
  - 

MembershipRenewalStatus

: Enum for membership renewal statuses.
- **Interfaces**
  - 

ILoanRepository

: Interface for loan repository.
  - 

ILoanService

: Interface for loan service.
  - 

IPatronRepository

: Interface for patron repository.
  - 

IPatronService

: Interface for patron service.
- **Services**
  - 

LoanService

: Implements loan-related operations.
  - 

PatronService

: Implements patron-related operations.

## Usage
1. Clone the repository.
2. Navigate to the 

Library.Console

 directory.
3. Run the application using the following command:
   ```sh
   dotnet run
   ```
4. Follow the on-screen instructions to interact with the library system.

## License
This project is licensed under the MIT License.