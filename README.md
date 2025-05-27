```
# Customer Complaint Form

A web application that provides a customer complaint form with full JavaScript validation. Users can submit detailed complaints about their orders and specify desired solutions. The form validates user input in real-time and on submission to ensure correctness and completeness.

---

## Features

- Validates full name is not empty.
- Validates email format.
- Validates order number to be a 10-digit number starting with "2024".
- Validates product code matches the pattern `XX##-X###-XX#` (letters and digits).
- Validates quantity is a positive integer.
- Requires at least one complaint checkbox selected.
- If "Other" complaint is selected, requires a detailed complaint description of at least 20 characters.
- Requires a solution radio button selected.
- If "Other" solution is selected, requires a detailed solution description of at least 20 characters.
- Provides real-time feedback with green/red borders on inputs, checkboxes, and radio groups.
- Highlights invalid fields on form submission.

---

## Installation

1. Clone or download this repository.

2. Open `index.html` in any modern browser (Chrome, Firefox, Edge, Safari).

3. No backend or build tools needed—pure HTML, CSS, and JavaScript.

---

## Usage

- Fill out all required fields in the complaint form.
- Real-time validation colors will guide you.
- Submit the form when all fields are valid.
- If invalid, fields with errors will be highlighted.
- On successful submission, the form resets and displays a success alert.

---

## File Structure

- `index.html` — The HTML markup for the form.
- `styles.css` — Stylesheet for form styling and validation feedback.
- `script.js` — JavaScript file implementing validation and form behavior.

---

## Validation Logic Summary

- **Full Name:** Must not be empty.
- **Email:** Must match a simple email regex pattern.
- **Order Number:** Must be exactly 10 digits starting with "2024".
- **Product Code:** Must match regex pattern `^[A-Za-z]{2}\d{2}-[A-Za-z]\d{3}-[A-Za-z]{2}\d$`.
- **Quantity:** Must be a positive integer greater than zero.
- **Complaints Group:** At least one checkbox checked.
- **Complaint Description:** Required if "Other" complaint is selected, minimum 20 characters.
- **Solutions Group:** Exactly one radio selected.
- **Solution Description:** Required if "Other" solution is selected, minimum 20 characters.

---

## How to Extend

- Replace alert messages with inline feedback messages.
- Enhance styles for better UX.
- Add backend integration to submit complaints to a server or database.
- Add CAPTCHA or spam protection.
- Localize validation messages.

---

## License

This project is open source and free to use.

---

## Contact

For questions or feedback, please contact me.
