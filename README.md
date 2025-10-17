# Installation Guide – ArtisanFind Project (Symfony)

## Prerequisites

Before starting, make sure you have the following installed:

* PHP ≥ 8.1
* Composer
* Symfony CLI
* MySQL (or XAMPP / another local server)

## Installation Steps

1. **Unzip the project**
   Unzip the `artisanfind.zip` archive into a directory of your choice:

```bash
cd path/to/your/project/artisanfind
```

2. **Install dependencies**

```bash
composer install
```

3. **Configure the database**
   Edit the `.env` or `.env.local` file and update the `DATABASE_URL` line:

```env
DATABASE_URL="mysql://username:password@127.0.0.1:3306/artisanfind_db?serverVersion=8.0"
```

4. **Create the database**

```bash
php bin/console doctrine:database:create
```

5. **Run migrations**

```bash
php bin/console doctrine:migrations:migrate
```

6. **Start the Symfony server**

```bash
symfony server:start
```

Then access the project at: [http://localhost:8000](http://localhost:8000)

---

## App Preview

<img width="498" height="223" alt="image" src="https://github.com/user-attachments/assets/090974b5-3293-4877-b6bc-a8e12304e18f" />
<img width="498" height="223" alt="image" src="https://github.com/user-attachments/assets/427ca37f-bfd6-4ec5-85ce-fcaeb077f058" />




## Developed by

**Ikram Sabir**
Engineering student at **Euromed University of Fez (EIDIA)**
