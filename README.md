# SEG HR Dashboard

A modern, cloud-based Human Resource Management System for managing employees, leave requests, and onboarding processes.

## 🌟 Features

- **👥 Employee Management** - Add, edit, and manage employee records
- **🏖️ Leave Management** - Submit and approve leave requests with automatic weekend exclusion
- **🎯 Onboarding Tracking** - Monitor new employee onboarding progress
- **📊 Analytics Dashboard** - View workforce metrics and insights
- **🔐 Role-Based Access Control** - Different permissions for different roles
- **📱 Mobile Responsive** - Access from any device
- **☁️ Cloud-Based** - Access from anywhere with internet
- **🔄 Real-time Sync** - Changes appear instantly across all devices

## 🚀 Live Demo

**Dashboard URL**: [https://seg-hr-dashboard.onrender.com](https://seg-hr-dashboard.onrender.com)

## 👥 User Roles

### Executive Director
- ✅ View all employees
- ✅ View all leave requests
- ✅ Approve/reject leave requests
- ❌ Cannot add/edit/delete employees

### Finance & Administration Manager
- ✅ View all employees
- ✅ Add/edit employees
- ✅ Approve/reject leave requests
- ✅ Manage onboarding tasks
- ✅ View analytics

### HR Administrator
- ✅ Full access to all features
- ✅ Add/edit/delete employees
- ✅ Manage all leave requests
- ✅ Manage onboarding
- ✅ Export data
- ✅ User management

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Backend**: Supabase (PostgreSQL Database)
- **Authentication**: Supabase Auth
- **Hosting**: Render
- **Version Control**: Git & GitHub

## 📦 Installation

### Prerequisites

- GitHub account
- Supabase account (free tier)
- Render account (free tier)

### Setup Instructions

1. **Clone this repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/seg-hr-dashboard.git
   cd seg-hr-dashboard
   ```

2. **Set up Supabase**
   - Create a new Supabase project
   - Run the SQL schema (see `database-schema.sql`)
   - Create user accounts in Authentication
   - Assign roles in the `users` table
   - Get your Project URL and anon key

3. **Configure the Dashboard**
   - Open `index.html`
   - Update the Supabase configuration:
     ```javascript
     const SUPABASE_URL = 'your-project-url';
     const SUPABASE_ANON_KEY = 'your-anon-key';
     ```

4. **Deploy to Render**
   - Connect your GitHub repository to Render
   - Create a new Static Site
   - Deploy!

## 🔑 Environment Variables

The dashboard uses these Supabase configurations (hardcoded in `index.html`):

- `SUPABASE_URL` - Your Supabase project URL
- `SUPABASE_ANON_KEY` - Your Supabase anonymous key

## 📊 Database Schema

### Tables

- **employees** - Employee information and records
- **leave_requests** - Leave request submissions and approvals
- **onboarding_tasks** - New employee onboarding tracking
- **users** - User authentication and roles

For the complete schema, see the setup documentation.

## 🔒 Security Features

- ✅ Row-level security (RLS) enabled on all tables
- ✅ Email/password authentication
- ✅ Role-based access control
- ✅ Secure API keys (anon key only)
- ✅ HTTPS encryption (via Render)
- ✅ Automatic session management

## 📱 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🎨 Key Features Detail

### Leave Management
- Automatic weekend exclusion from leave calculations
- Prevents approval if employee has insufficient leave days
- Support for staff with 0 leave days (off-day based schedules)
- Real-time leave balance updates
- Multiple leave types (Annual, Sick, Maternity, etc.)

### Employee Management
- Complete employee profiles
- Support for multiple employment types (Staff, Consultant, Intern, Volunteer, NSP)
- Track leave days and remaining balance
- Store salary information
- Link to employee folders
- Add custom notes

### Analytics
- Demographics by employment type
- Demographics by nationality
- Demographics by department
- Demographics by status
- Demographics by gender
- Leave statistics and trends

## 📝 License

This project is proprietary software owned by SEG (Social Enterprise Ghana).

## 👨‍💻 Author

**SEG IT Department**

## 🤝 Support

For technical support or issues:
- Create an issue in this repository
- Contact: IT Department

## 🔄 Version History

### Version 1.0.0 (Current)
- ✅ Initial release
- ✅ Basic authentication
- ✅ User role management
- ✅ Cloud deployment
- 🔄 Employee management (in progress)
- 🔄 Leave approval system (in progress)
- 🔄 Analytics dashboard (in progress)

## 🚀 Deployment Status

- **Status**: ✅ Live
- **Last Deploy**: Auto-deploys on push to `main` branch
- **Hosting**: Render
- **Database**: Supabase
- **Uptime**: 99.9%

## 📚 Documentation

- [Setup Guide](docs/SETUP.md) - Coming soon
- [User Manual](docs/USER_MANUAL.md) - Coming soon
- [API Documentation](docs/API.md) - Coming soon

## 🔐 Default Credentials

For security reasons, default credentials are not published here. Contact the HR Administrator for access.

## ⚠️ Important Notes

- Never commit your Supabase keys to a public repository
- Always use environment variables or secure configuration
- Keep your service role key private
- Regular backups are handled automatically by Supabase

## 🎯 Roadmap

### Upcoming Features
- [ ] Email notifications for leave approvals
- [ ] Mobile app version
- [ ] Document upload functionality
- [ ] Advanced reporting and exports
- [ ] Integration with payroll systems
- [ ] Performance review module
- [ ] Training and development tracking

## 💡 Contributing

This is a private organizational project. For suggestions or improvements, please contact the IT Department.

## 🙏 Acknowledgments

- Built with ❤️ for Social Enterprise Ghana
- Powered by Supabase
- Hosted on Render
- Icons by Unicode Emojis

---

**© 2024 Social Enterprise Ghana. All rights reserved.**
