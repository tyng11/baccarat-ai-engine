# Baccarat AI Ensemble Engine

## Dashboard Access

Visit the main dashboard: `index.html`

## Admin Panel

Access the admin panel at: `admin.html`

### Admin Features

- **Master Password**: `admin123` (Change this immediately in admin.html)
- **Password Management**: Add, delete, and activate member access codes
- **Rotation Schedules**:
  - **Daily**: Passwords rotate every 24 hours
  - **Weekly**: Passwords rotate every 7 days
  - **Bi-Weekly**: Passwords rotate every 14 days
  - **Static**: No automatic rotation

### Quick Start

1. Open `admin.html` in your browser
2. Login with the master password: `admin123`
3. Add new 5-digit passwords with your desired rotation schedule
4. Passwords automatically sync to the main dashboard
5. Monitor all activity in the Activity Log

### How It Works

- **LocalStorage**: All passwords and settings are stored in your browser's localStorage
- **Session Management**: Admin session persists during your browser session
- **Auto-Sync**: Any changes automatically update the main dashboard
- **Activity Logging**: All actions are logged with timestamps

### Security Notes

⚠️ **This is a client-side implementation**. For production use:
- Store passwords securely on a backend server
- Use HTTPS for all communications
- Implement proper authentication and authorization
- Use hashed passwords, never plain text

### Customization

**To change the master admin password:**

Edit `admin.html` line ~78:
```javascript
const MASTER_ADMIN_PASSWORD = "admin123"; // Change this
```

**To set initial passwords:**

Modify the localStorage data in your browser console or add to the page initialization.
