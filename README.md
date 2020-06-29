### LIBRARY MANAGMENT API

## INSTALLATION

### Installing Dependencies

Run
`npm i`

### .env
Create a .env file in the root directory and paste in this

```
MONGO_URI=
JWT_SECRET=
SMTP_HOST=
SMTP_PORT=
SENDGRID_USER=
SENDGRID_PASS=
ADMIN_NAME=
ADMIN_PASS=
```

## Routes Menu

### Admin
- [Admin Login](#1-admin-login-post-request)

### 1. Admin Login: POST Request

End Point
```
/api/v1/admin/login
```

Body
```json
{
	"username": "admin",
	"password": "admin1234"
}
```

Response
```json
{
    "status": 200,
    "message": "Logged in successfully",
    "data": {
        "username": "admin",
        "role": "admin",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6ImFkbWluIiwicGFzc3dvcmQiOiJhZG1pbjEyMzQiLCJyb2xlIjoiYWRtaW4iLCJpYXQiOjE1OTM0NTgxODF9._px-XcaM1TrAuVHy_dmrXe8TlfDMunyHaQRGf7BzHdQ"
    }
}
```