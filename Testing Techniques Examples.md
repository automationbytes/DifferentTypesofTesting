# Testing Techniques Examples

## Equivalence Class Partitioning (ECP) and Boundary Value Analysis (BVA) for User Name

### Example case
 - The User Name should only accept lowercase letters (a-z) and must be between 6 to 8 characters long.

### Equivalence Class Partitioning (ECP)

**Description:** Equivalence Class Partitioning divides input data into valid and invalid partitions to ensure comprehensive testing.

**Example:**
- **Valid Partition:**
  - **Lowercase letters (a...z):**
    - User name containing only lowercase letters is considered valid.

- **Invalid Partitions:**
  - **Uppercase letters (A...Z):**
    - User name containing any uppercase letters is invalid.
  - **Numbers (0...9):**
    - User name containing any numeric characters is invalid.
  - **Special characters (@, #, $, &, etc.):**
    - User name containing any special characters is invalid.
  - **Empty Characters:**
    - User name containing only empty characters (spaces, tabs) is invalid.

### Boundary Value Analysis (BVA)

**Description:** Boundary Value Analysis tests the boundaries between valid and invalid input values.

**Example:**
- **Parameters and Values:**
  - Minimum length: 6 characters
  - Maximum length: 8 characters

**Test Cases:**
1. **Min (6 characters):** Valid
2. **Min+1 (7 characters):** Valid
3. **Min-1 (5 characters):** Invalid
4. **Max (8 characters):** Valid
5. **Max+1 (9 characters):** Invalid
6. **Max-1 (7 characters):** Valid
7. **Empty characters only:** Invalid

**Result:**
- Min (6 characters): Valid
- Min+1 (7 characters): Valid
- Min-1 (5 characters): Invalid
- Max (8 characters): Valid
- Max+1 (9 characters): Invalid
- Max-1 (7 characters): Valid
- Empty characters only: Invalid

## Decision Table Testing

**Description:** Decision Table Testing uses a table to represent combinations of inputs and their corresponding outputs.

**Example:**
For a simple login form with conditions:
- Valid username: "user1"
- Valid password: "password1"

**Decision Table:**

| Condition                   | Rule 1 | Rule 2 | Rule 3 | Rule 4 | Rule 5 |
|-----------------------------|--------|--------|--------|--------|--------|
| Username = "user1"          | T      | T      | F      | F      | F      |
| Password = "password1"      | T      | F      | T      | F      | T      |
| Empty Characters            | F      | F      | F      | F      | T      |
| Output (Login Successful)   | Yes    | No     | No     | No     | No     |

**Test Cases:**
1. Input: Username = "user1", Password = "password1" (Login Successful)
2. Input: Username = "user1", Password = "wrongpassword" (Login Failed)
3. Input: Username = "wronguser", Password = "password1" (Login Failed)
4. Input: Username = "wronguser", Password = "wrongpassword" (Login Failed)
5. Input: Username = "", Password = "" (Login Failed)
