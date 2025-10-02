# User Profile GUI Application

## Overview
This Java Swing application allows users to create a personal profile by entering their details and optionally uploading a profile photo. The program validates the input and displays the created profile in a popup, including the uploaded photo if provided.

The project is organized into two packages:
- `model` – Contains the `User` class representing the user profile.
- `ui` – Contains the `UserJFrame` class, the GUI for input and displaying user information.

---

## Features
- Input fields for:
  - First Name
  - Last Name
  - Gender (Male, Female, Other)
  - Age
  - Phone Number
  - Email
  - Continent
  - Hobbies
- Upload a profile photo (`jpg`, `png`, `jpeg`)
- Input validation:
  - Required fields must not be empty
  - Phone number must be at least 8 digits
  - Email format must be valid
- Displays a success popup with user information and photo

---

## File Structure

### `model/User.java`
- Represents a user profile.
- Contains:
  - Private instance variables for all profile fields, including optional photo
  - Constructor for initializing all fields
  - Getters and setters
  - `toString()` method to display user information (excluding the photo)

### `ui/UserJFrame.java`
- GUI form for creating and displaying user profiles.
- Features:
  - Input fields for all user data
  - Buttons to upload a photo and submit the form
  - Validation logic for required fields, phone number, and email
  - Creates a `User` object and shows profile details in a popup
  - Shows the uploaded photo in the popup if available

---

## How to Run
1. Open the project in NetBeans or any Java IDE.
2. Ensure the packages `model` and `ui` are correctly structured.
3. Compile the project.
4. Run `ui.UserJFrame`.
5. Enter user information, optionally upload a photo, and click **Submit**.
6. A popup will display the user's profile information and the uploaded photo (if any).

---

## Validation Rules
- First Name, Last Name, Phone, and Email are required.
- Phone must contain at least 8 digits.
- Email must follow a valid format (e.g., `user@example.com`).

---

## Dependencies
- Java SE 8 or higher
- Swing (built-in Java GUI library)

---

## Notes
- Uses `JFileChooser` for photo upload.
- Uses `JOptionPane` to display messages and user profile.
- `User` stores the uploaded photo as a `File` object for potential future use (e.g., saving or editing).

---
## Screenshot
The Screenshot folder contains visual references of the application’s interface and functionality. These images demonstrate different stages of using the User Profile GUI Application, including form input, validation, and the profile display popup.
File Naming Convention: Each screenshot is automatically named with a timestamp (e.g., Screenshot 2025-10-02 at 10.12.35 AM.png).
Content:
Application startup window
User input form
Profile creation and validation steps
Popup window showing profile details and uploaded photo
These screenshots serve as a guide for understanding how the application looks and behaves during execution.

## Author
- Oseme Edeoghon
- Ishmael Otchere
