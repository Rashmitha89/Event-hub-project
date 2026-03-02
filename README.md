# Campus EventHub 

**Campus EventHub** is a modern, responsive web application designed for university students and administrators to manage and discover campus events seamlessly. 

---

##  Features

### For Students (Viewers):
- **Event Discovery**: Browse through "New" and "Ongoing" campus events.
- **Search & Filter**: Quickly find events by title or category.
- **Real-time Updates**: See the latest event details instantly.
- **RSVP System**: Register for events with a single click.
- **Feedback & Ratings**: Rate and review events to share your experience.

### For Administrators:
- **Comprehensive Dashboard**: View key metrics (Total Events, RSVPs, Feedback).
- **Event Management**: Create, Update, and Delete event listings.
- **Registration Control**: Approve or manage student RSVPs.
- **Feedback Analysis**: View user reviews grouped by event for better insights.
- **Role-Based Security**: Secure access to the Admin Panel.

---

##  Tech Stack

- **Frontend**: Blazor WebAssembly (.NET 8.0)
- **Database & Auth**: Firebase Firestore & Firebase Authentication
- **Styling**: Bootstrap 5 + Vanilla CSS
- **Icons**: Bootstrap Icons

---

##  Setup Instructions

### Prerequisites
1. **.NET 8.0 SDK** installed.
2. **Visual Studio 2022** or **VS Code**.
3. A **Firebase Project** (Google Account required).

### Steps to Run Locally

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd BookAPP
   ```

2. **Configure Firebase**:
   - Go to the [Firebase Console](https://console.firebase.google.com/).
   - Create a new project.
   - Register a "Web App" and copy the `firebaseConfig` object.
   - Open `wwwroot/index.html` and replace the existing `firebaseConfig` with your own.

3. **Set Up Database Rules**:
   - In Firestore, set up a collection named `events`, `rsvps`, and `feedback`.
   - Ensure the security rules allow read/write access based on your requirements.

4. **Run the Application**:
   - Open the solution in Visual Studio.
   - Press **F5** or run:
     ```bash
     dotnet run
     ```
   - The app will be available at `http://localhost:5245`.

###  Admin Credentials (Default for Testing)
- **Email**: `admin`
- **Password**: `1234`
*(Note: These are hardcoded for local testing in `index.html`)*

---

##  License
This project is for educational purposes as part of a university assignment.
