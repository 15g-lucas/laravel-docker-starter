# Laravel Starter Project

**A Dockerized Laravel development environment**

### **Installation**
1. **Clone the Repository:**
   ```bash
   git clone <https://github.com/15g-lucas/laravel-docker-starter.git>
   ```
2. **Install Dependencies:**
   ```bash
   composer install
   npm install
   ```
3. **Configure Environment:**
    - Copy the `.env.example` file to `.env` and customize it with your desired database credentials.
   ```bash
   cp .env.example .env
   ```
4. **Start Development Environment:**
   ```bash
   docker-compose up -d --build
   ```

### **Customization**

#### **.env File**
* **Customize database credentials:** Modify the `.env` file with your preferred database settings:
  ```
  DB_DATABASE=your_database
  DB_USERNAME=your_username
  DB_PASSWORD=your_password
  ```
* **Other environment variables:** You can define additional environment variables as needed for your application, such as API keys, application URLs, etc.

#### **docker-compose.yml**
* **Services:** Customize the services (e.g., add a mailhog service for testing emails).
* **Networks:** Define additional networks for communication between services.
* **Volumes:** Mount additional volumes to persist data.

### **Connecting to the Container**
```bash
docker exec -it laravel_app bash
```
