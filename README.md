# Running project

## 1. Create .env file

```
cp .env.example .env
```

## 2. Start docker containers using Sail

```
sail up
```

## 3. Install dependencies

```
sail composer install
```

## 4. Migrate and seed database

```
sail artisan migrate:fresh --seed
```

## 5. Log into admin panel in browser

Open admin panel in browser:

```
http://localhost:8080/admin/login
```

Login with test user data:

User: `test@example.com`
Password: `password`

## 6. Create new category

Click on the Categories on the sidebar and create new category. After it is created you will see relation manager. Try to attach sample product it will fail when you try to search for products.
