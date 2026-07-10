# XeroLogin

A simple clean register and login plugin for Paper 1.21.11 servers by **XeroDev**

---

## What it does

- New players see a blue **REGISTER** title with white subtext  
  `Type /register <password> <repeat>`
- Registered players see a blue **LOGIN** title with white subtext  
  `Type /login <password> to login`
- No persistent sessions by default — every join requires `/login` again  
  Sessions are optional and configurable in `config.yml`
- While unauthenticated players are frozen — no movement no chat no commands except `/register` and `/login` (all configurable)

---

## Commands

| Command | Description |
|---------|-------------|
| `/register <password> <repeat>` | Create your account |
| `/login <password>` | Log in |
| `/logout` | Log out manually |
| `/changepassword <old> <new>` | Change your password |
| `/xerologin reload` | Reload config.yml |
| `/xerologin changepass <player> <newPassword>` | Admin force‑change a password |
| `/xerologin unregister <player>` | Admin wipe an account so it can register again |

Admin commands require the `xerologin.admin` permission (OP by default)

---

## Configuration

Edit `config.yml` to change messages and titles toggle sessions set min and max password length and control what is blocked before login

---

## Building it yourself

1. Install JDK 21 and Gradle
