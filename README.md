# git-social
Git Social is a social media platform designed exclusively for programmers. Built with Django, it offers a space for developers to connect, collaborate, and share their coding journey. Whether it's sharing projects, discussing ideas, or showcasing skills, Git-Social brings the developer community closer together.

---

## 🚀 Features

- **Profile Customization**: Create a unique developer profile with links to your GitHub, portfolio, and more.
- **Project Sharing**: Share your repositories, side projects, and coding milestones with the community.
- **Discussion Forums**: Engage in meaningful discussions, ask questions, and share knowledge.
- **Follow & Interact**: Follow fellow programmers, like their posts, and leave comments.
- **Tech Stack Highlighting**: Showcase the technologies you use and love.
- **Dark Mode**: Enjoy a sleek dark mode for late-night coding sessions.

---

## 🛠️ Tech Stack

- **Backend**: Django 5.x
- **Frontend**: Django Templates, Bootstrap (optional: Tailwind for advanced customization)
- **Database**: SQLite (for development), PostgreSQL (recommended for production)
- **Authentication**: Django’s built-in authentication system with social login (e.g., GitHub OAuth)
- **APIs**: REST API for future mobile or third-party integrations (via Django REST Framework)

---

## 📦 Installation and Setup

### Prerequisites
- Python 3.10+
- Node.js (if using a modern CSS framework like Tailwind)
- PostgreSQL (optional for production)

### 1. Clone the Repository
```bash
git clone https://github.com/V-FOR-VEND3TTA/git-social.git
cd git-social
```

### 2. Create a Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install django django-allauth psycopg2-binary djangorestframework
```

### 4. Configure Environment Variables
Create a `.env` file in the root directory with the following:
```env
SECRET_KEY=your_secret_key
DEBUG=True
DATABASE_URL=sqlite:///db.sqlite3 # Update to Postgres for production
GITHUB_CLIENT_ID=your_github_client_id
GITHUB_CLIENT_SECRET=your_github_client_secret
```

### 5. Apply Migrations
```bash
python manage.py migrate
```

### 6. Run the Development Server
```bash
python manage.py runserver
```

---

## 🎨 Optional: Tailwind CSS Setup
If you want to enhance the UI with Tailwind CSS, follow these steps:

1. Install Tailwind CSS:
   ```bash
   npm install -D tailwindcss postcss autoprefixer
   npx tailwindcss init
   ```

2. Configure `tailwind.config.js` to include your Django templates:
   ```javascript
   module.exports = {
       content: ['./**/*.html'],
       theme: {
           extend: {},
       },
       plugins: [],
   };
   ```

3. Run Tailwind in watch mode:
   ```bash
   npm run dev
   ```

---

## 🌟 Future Enhancements

- Real-time chat feature using WebSockets (e.g., Django Channels).
- Advanced search functionality to find developers by skillset, location, or interests.
- Integration with popular code repositories (e.g., GitHub, GitLab, Bitbucket).
- User badges and achievements for contributing to the community.
- REST API for external integrations and mobile apps.

---

## 🛡️ Deployment

1. Configure production settings in `settings.py`.
2. Use platforms like Heroku, Vercel, or Docker for deployment.
3. Use a PostgreSQL database for production.

---

## 📜 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## 🧑‍💻 Contributing
We welcome contributions from the community! To contribute:
1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m "Add feature"`.
4. Push to the branch: `git push origin feature-name`.
5. Open a pull request.

---

## 🌟 Acknowledgments

- [Django](https://www.djangoproject.com/)
- [Django-Allauth](https://django-allauth.readthedocs.io/en/latest/)
- [Django REST Framework](https://www.django-rest-framework.org/)
- [GitHub OAuth](https://docs.github.com/en/developers/apps/building-oauth-apps)

---

## 📞 Contact
For questions or suggestions:
- **Email**: [georgehlongwane8@gmail.com](mailto:georgehlongwane8@gmail.com)
- **GitHub**: [V-FOR-VEND3TTA](https://github.com/V-FOR-VEND3TTA)

---
