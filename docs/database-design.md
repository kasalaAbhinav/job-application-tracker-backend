# Database Design

## User Table

| Column | Type | Description |
|---|---|---|
| id | Long | Primary key |
| name | String | User full name |
| email | String | User email |
| password | String | Encrypted password |

## Job Application Table

| Column | Type | Description |
|---|---|---|
| id | Long | Primary key |
| companyName | String | Company name |
| role | String | Job role |
| status | String | Application status |
| appliedDate | LocalDate | Date of application |
| deadline | LocalDate | Last date or follow-up date |
| jobLink | String | Job posting link |
| notes | String | Personal notes |
| userId | Long | Foreign key to User table |

## Status Values

- APPLIED
- SHORTLISTED
- INTERVIEW
- OFFER
- REJECTED