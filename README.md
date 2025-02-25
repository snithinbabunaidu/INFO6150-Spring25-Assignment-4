# INFO6150-Spring25-Assignment-4 (Form Validation Assignment)

## Overview
This project implements a dynamic feedback form with real-time validation, input masking, and data submission functionality. The form includes various input types and implements specific validation rules for each field.

## Features

### Form Validations![ss3](https://github.com/user-attachments/assets/61447c36-2f08-404e-9de5-108ab9b8a473)
![ss2](https://github.com/user-attachments/assets/cf0079f9-43aa-42d8-8ff0-eefe47e45a29)
![assignment4](https://github.com/user-attachments/assets/33aa522a-5d89-4a1c-8e71-2a71b0210410)
![ss4](https://github.com/user-attachments/assets/b031784a-0997-426f-bfe6-adcaffa5e2a5)

- All mandatory fields marked with asterisk (*)
- Real-time validation on key events
- Custom validation rules:
  - First/Last Name: 2-30 alphanumeric characters
  - Email: Must be @northeastern.edu domain
  - Phone: (XXX) XXX-XXXX format with input masking
  - Zipcode: 5-digit validation
  - Street Address 1: Minimum 2 characters
  - Dynamic error highlighting with red text

### Dynamic Features
- Input masking for phone numbers
- Live character counter for Street Address 2 field (20 characters max)
- Dynamic checkbox generation based on dropdown selection
- Conditional text fields appear when checkboxes are selected

### Submission Handling
- Submit button disabled until all validations pass
- Data displayed in a table below the form
- Previous submissions retained and displayed
- Form fields cleared after successful submission

## Technical Implementation

### Key Components
1. **Form Validation**
   - Regex patterns for field validation
   - Real-time error messaging
   - Custom validation for dynamic fields

2. **Input Masking**
   - Phone number formatting: (XXX) XXX-XXXX
   - Automatic formatting while typing

3. **Dynamic Elements**
   - Dropdown-triggered checkbox generation
   - Conditional text field display
   - Character counter implementation

4. **Data Management**
   - Form data collection and validation
   - Submission storage and display
   - Table generation and updates

### File Structure
```
- form.html (contains HTML, CSS, and JavaScript)
```

## Usage

### Required Fields
- Title (Miss/Mr./Mrs.)
- First Name
- Last Name
- Email (@northeastern.edu)
- Phone Number
- Zipcode
- Street Address 1
- How did you hear (with dynamic options)
- Comments

### Optional Fields
- Street Address 2 (with character counter)

## Local Development
1. Clone the repository
2. Open index.html in a web browser
3. No additional setup or dependencies required

## Browser Compatibility
- Tested on modern browsers (Chrome, Firefox, Safari)
- Uses standard JavaScript features
- No external libraries required

## Notes
- All validations occur in real-time
- Form data persists until page refresh
- Table styling optimized for readability
- Error messages are context-specific

## Future Enhancements
- Add form data persistence using localStorage
- Implement edit/delete functionality for submitted entries
- Add form data export feature
- Enhance mobile responsiveness
