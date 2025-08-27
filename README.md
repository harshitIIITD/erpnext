<div align="center">
    <a href="https://github.com/harshitIIITD/erpnext">
	<img src="./erpnext/public/images/v16/erpnext.svg" alt="FashionFlow Logo" height="80px" width="80xp"/>
    </a>
    <h2>FashionFlow</h2>
    <p align="center">
        <p>Powerful, Intuitive Fashion Industry Management System</p>
    </p>

[![Fashion Industry ERP](https://img.shields.io/badge/Fashion-Industry%20ERP-purple?style=flat-square)](https://github.com/harshitIIITD/erpnext)<br><br>
[![Open Source](https://img.shields.io/badge/Open%20Source-Fashion%20Management-green?style=flat-square)](https://github.com/harshitIIITD/erpnext)

</div>

<div align="center">
	<img src="./erpnext/public/images/v16/hero_image.png"/>
</div>

<div align="center">
	<a href="https://github.com/harshitIIITD/erpnext">Repository</a>
	-
	<a href="https://github.com/harshitIIITD/erpnext/issues">Issues</a>
	-
	<a href="https://github.com/harshitIIITD/erpnext/blob/develop/README.md">Documentation</a>
</div>

## FashionFlow

100% Open-Source Fashion Industry Management System to streamline your fashion business operations.

### Motivation

Running a fashion business involves complex challenges - managing designs, tracking fabric inventory, handling production schedules, customer orders, seasonal collections, and supplier relationships. In an industry where software solutions are fragmented and expensive, FashionFlow provides a comprehensive, integrated platform that addresses all these needs and more, for free.

### Key Features

- **Fashion Accounting**: Specialized financial management for fashion businesses including seasonal budgeting, collection costing, and fashion-specific reporting.
- **Collection Management**: Plan, design, and track fashion collections from concept to retail, managing SKUs, variants, colors, and sizes.
- **Fabric & Material Sourcing**: Track fabric inventory, manage supplier relationships, handle purchase orders for materials, and monitor quality standards.
- **Production Management**: Streamline garment manufacturing from cutting to finishing, track work orders, manage subcontractors, and monitor production timelines.
- **Retail Operations**: Handle customer orders, manage boutique inventory, process returns, and track sales across multiple channels.
- **Fashion Projects**: Manage fashion shows, photo shoots, marketing campaigns, and seasonal launches with integrated project management tools.

<details open>

<summary>Fashion Industry Screenshots</summary>
	<p><em>Screenshots showing fashion-specific features like collection management, fabric tracking, and production planning would be displayed here in a production environment.</em></p>
</details>

### Under the Hood

- [**Frappe Framework**](https://github.com/frappe/frappe): A full-stack web application framework written in Python and Javascript. The framework provides a robust foundation for building web applications, including a database abstraction layer, user authentication, and a REST API.

- [**Frappe UI**](https://github.com/frappe/frappe-ui): A Vue-based UI library, to provide a modern user interface. The Frappe UI library provides a variety of components that can be used to build single-page applications on top of the Frappe Framework.

## Production Setup

### Self-Hosted
#### Docker

Prerequisites: docker, docker-compose, git. Refer [Docker Documentation](https://docs.docker.com) for more details on Docker setup.

Run following commands:

```
git clone https://github.com/frappe/frappe_docker
cd frappe_docker
docker compose -f pwd.yml up -d
```

After a couple of minutes, site should be accessible on your localhost port: 8080. Use below default login credentials to access the site.
- Username: Administrator
- Password: admin

See [Frappe Docker](https://github.com/frappe/frappe_docker?tab=readme-ov-file#to-run-on-arm64-architecture-follow-this-instructions) for ARM based docker setup.


## Development Setup
### Manual Install

The Easy Way: our install script for bench will install all dependencies (e.g. MariaDB). See https://github.com/frappe/bench for more details.

New passwords will be created for the FashionFlow "Administrator" user, the MariaDB root user, and the frappe user (the script displays the passwords and saves them to ~/frappe_passwords.txt).


### Local

To setup the repository locally follow the steps mentioned below:

1. Setup bench by following the [Installation Steps](https://frappeframework.com/docs/user/en/installation) and start the server
   ```
   bench start
   ```

2. In a separate terminal window, run the following commands:
   ```
   # Create a new site
   bench new-site fashionflow.localhost
   ```

3. Get the FashionFlow app and install it
   ```
   # Get the FashionFlow app
   bench get-app https://github.com/harshitIIITD/erpnext

   # Install the app
   bench --site fashionflow.localhost install-app fashionflow
   ```

4. Open the URL `http://fashionflow.localhost:8000/app` in your browser, you should see the app running

## Learning and community

1. [Frappe School](https://school.frappe.io) - Learn Frappe Framework fundamentals for building business applications.
2. [GitHub Repository](https://github.com/harshitIIITD/erpnext) - Browse the source code and documentation for FashionFlow.
3. [GitHub Issues](https://github.com/harshitIIITD/erpnext/issues) - Report bugs and request new fashion industry features.
4. [Fashion Industry Resources](https://github.com/harshitIIITD/erpnext) - Access fashion-specific guides and tutorials.


## Contributing

1. [Issue Guidelines](https://github.com/harshitIIITD/erpnext/issues)
2. [Report Security Vulnerabilities](https://github.com/harshitIIITD/erpnext/security)
3. [Pull Request Requirements](https://github.com/harshitIIITD/erpnext/pulls)
4. [Fashion Industry Translations](https://github.com/harshitIIITD/erpnext)


## Logo and Trademark Policy

Please read our [Logo and Trademark Policy](TRADEMARK_POLICY.md).

<br />
<br />
<div align="center" style="padding-top: 0.75rem;">
	<a href="https://github.com/harshitIIITD/erpnext" target="_blank">
		<span style="font-weight: bold; color: #8e44ad;">FashionFlow</span> - Fashion Industry Management System
	</a>
</div>
