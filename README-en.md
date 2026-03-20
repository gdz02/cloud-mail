<p align="center">
    <img src="doc/demo/logo.png" width="80px" />
    <h1 align="center">PostLite</h1>
    <p align="center">A high-performance lightweight mail system built for teams, with full send/receive workflow and Linux readiness 🎉</p> 
    <p align="center">
       <a href="/README.md" style="margin-left: 5px">简体中文</a> | English 
    </p>
    <p align="center">
        <a href="https://github.com/postlite/postlite/tree/main?tab=MIT-1-ov-file" target="_blank" >
            <img src="https://img.shields.io/badge/license-MIT-green" />
        </a>    
        <a href="https://github.com/postlite/postlite/releases" target="_blank" >
            <img src="https://img.shields.io/github/v/release/postlite/postlite" alt="releases" />
        </a>  
        <a href="https://github.com/postlite/postlite/issues" >
            <img src="https://img.shields.io/github/issues/postlite/postlite" alt="issues" />
        </a>  
        <a href="https://github.com/postlite/postlite/stargazers" target="_blank">
            <img src="https://img.shields.io/github/stars/postlite/postlite" alt="stargazers" />
        </a>  
        <a href="https://github.com/postlite/postlite/forks" target="_blank" >
            <img src="https://img.shields.io/github/forks/postlite/postlite" alt="forks" />
        </a>
    </p>
    <p align="center">
        <a href="https://trendshift.io/repositories/14418" target="_blank" >
            <img src="https://trendshift.io/api/badge/repositories/14418" alt="trendshift" >
        </a>
    </p>
</p>

## Description
With one domain, you can create multiple email addresses like mainstream mail platforms. PostLite focuses on high performance and lightweight operations, and is ready for Linux server deployments for team use.
## Project Showcase

- [Live Demo](https://skymail.ink)<br>
- [Deployment Guide](https://doc.skymail.ink/en/)<br>


| ![](/doc/demo/demo1.png) | ![](/doc/demo/demo2.png) |
|--------------------------|--------------------------|
| ![](/doc/demo/demo3.png) | ![](/doc/demo/demo4.png) |

## Features

- **💰 Low-Cost Usage**: Deploy on Linux servers to reduce team infrastructure and maintenance costs.

- **💻 Responsive Design**: Automatically adapts to both desktop and most mobile browsers.

- **📧 Email Sending**: Integrated with Resend, supporting bulk email sending and attachments.

- **🛡️ Admin Features**: Admin controls for user and email management with RBAC-based access control.

- **📦 Attachment Support**: Send and receive attachments, stored and downloaded via internal object storage.

- **🔔 Email Push**: Forward received emails to Telegram bots or other email providers.

- **📡 Open API**: Supports batch user creation via API and multi-condition email queries

- **📈 Data Visualization**: Use ECharts to visualize system data, including user email growth.

- **🎨 Personalization**: Customize website title, login background, and transparency.

- **🤖 CAPTCHA**: Integrated with Turnstile CAPTCHA to prevent automated registration.

- **📜 More Features**: Under development...

## Tech Stack

- **Platform**: Linux servers (bare metal / VM / cloud instances)

- **Web Framework**: [Hono](https://hono.dev/)

- **ORM**: [Drizzle](https://orm.drizzle.team/)

- **Frontend Framework**: [Vue3](https://vuejs.org/)

- **UI Framework**: [Element Plus](https://element-plus.org/)

- **Email Service**: [Resend](https://resend.com/)

- **Cache**: Built-in cache module

- **Database**: Built-in database module

- **File Storage**: Built-in object storage module

## Project Structure

```
postlite
├── mail-worker				    # Backend worker project
│   ├── src                  
│   │   ├── api	 			    # API layer
│   │   ├── const  			    # Project constants
│   │   ├── dao                 # Data access layer
│   │   ├── email			    # Email processing and handling
│   │   ├── entity			    # Database entities
│   │   ├── error			    # Custom exceptions
│   │   ├── hono			    # Web framework, middleware, error handling
│   │   ├── i18n			    # Internationalization
│   │   ├── init			    # Database and cache initialization
│   │   ├── model			    # Response data models
│   │   ├── security			# Authentication and authorization
│   │   ├── service			    # Business logic layer
│   │   ├── template			# Message templates
│   │   ├── utils			    # Utility functions
│   │   └── index.js			# Entry point
│   ├── package.json			# Project dependencies
│   └── wrangler.toml			# Project configuration
│
├─ mail-vue				        # Frontend Vue project
│   ├── src
│   │   ├── axios 			    # Axios configuration
│   │   ├── components			# Custom components
│   │   ├── echarts			    # ECharts integration
│   │   ├── i18n			    # Internationalization
│   │   ├── init			    # Startup initialization
│   │   ├── layout			    # Main layout components
│   │   ├── perm			    # Permissions and access control
│   │   ├── request			    # API request layer
│   │   ├── router			    # Router configuration
│   │   ├── store			    # Global state management
│   │   ├── utils			    # Utility functions
│   │   ├── views			    # Page components
│   │   ├── app.vue			    # Root component
│   │   ├── main.js			    # Entry JS file
│   │   └── style.css			# Global styles
│   ├── package.json			# Project dependencies
└── └── env.release				# Environment configuration

```

## Support

<a href="https://doc.skymail.ink/support.html">
<img width="170px" src="./doc/images/support.png" alt="">
</a>

## License

This project is licensed under the [MIT](LICENSE) license.

## Communication

[Telegram](https://t.me/cloud_mail_tg)
