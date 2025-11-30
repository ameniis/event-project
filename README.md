# 📌 Events Project -- Symfony Application

This README explains how to set up the project on any machine, so
everyone can contribute without errors.

------------------------------------------------------------------------

# 🚀 Getting Started

## ✅ 1. Clone the Repository

    git clone https://github.com/ameni/events-project.git
    cd events-project


------------------------------------------------------------------------

# 📦 Install Project Dependencies

## ✅ 2. Install Composer Dependencies

    composer install

This recreates the `vendor/` folder.

------------------------------------------------------------------------

# 🛠 Environment Configuration

## ✅ 3. Configure the `.env` File

Open the `.env` file and set your database URL:

    DATABASE_URL="mysql://root:Passw@rd2002@127.0.0.1:3306/events"

------------------------------------------------------------------------

# 🗄 Database Setup

## ✅ 4. Create the Database

    php bin/console doctrine:database:create

## ✅ 5. Run Migrations

    php bin/console doctrine:migrations:migrate

------------------------------------------------------------------------

# ▶️ Run the Project

## ✅ Start Symfony Local Server

If you have Symfony CLI installed:

    symfony serve

Otherwise:

    php -S localhost:8000 -t public

Open the browser at:

    http://127.0.0.1:8000

------------------------------------------------------------------------

# 👥 Team Workflow

## Branching Strategy

Each team member should create a branch for their feature:

    git checkout -b feature-name

After finishing work:

    git add .
    git commit -m "Add feature"
    git push origin feature-name

Then open a Pull Request on GitHub.

------------------------------------------------------------------------

# 📝 Entities Included

### ✔ Review

User review for an event (rating + comment).

### ✔ Notification

A message sent to a user (read/unread).

------------------------------------------------------------------------
