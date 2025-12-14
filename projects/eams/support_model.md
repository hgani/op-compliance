Last modified: 9 Dec 2025

## Overview

This document outlines our proposed support package for the initial launch (MVP) of the Emergency Accommodation Management System (EAMS).

## Maintenance

- Under this support model, we will maintain the system for bug fixes and security patches.

- We will ensure the system and its dependencies are kept up to date to maintain extensibility, modifiability, and upgradability, without requiring a full system rebuild in the future.

  - When properly maintained, system updates and upgrades are typically low-risk.

- We will also handle monitoring and maintenance of the underlying Azure infrastructure.

## Infrastructure and Services

- This support package also covers the infrastructure costs (e.g., Azure, Github) for three Azure environments: production, staging, and development.

- In addition to server infrastructure, it covers the services required for the MVP to function, which include:

  - Google place data and photos

  - Google maps

  - Email sending

  - Photo and document storage

  - Entra ID

## Modifications

- We provide minor tweaks at no additional cost, such as updating text, changing colours, replacing logos, etc.

- In addition, we can add or remove categories, such as client groups and accommodation attributes, as long as it does not add complexity to the filtering and displaying logic.

  - However, this does not include nearby service categories, as these often require significant effort due to external API limitations and quirks (e.g., Google Place API).

- Enhancements are not included as part of maintenance.

  - This refers to the development of new functionality.

  - However, we are happy to offer free consultation and recommendations on cost-effective solutions to meet new requirements or address specific challenges.

## Maintenance Support Pricing

- Our maintenance support is priced at **$4,600 plus GST per month**.

  - This price includes all Infrastructure and Services costs, as well as the Maintenance and Modifications work mentioned above.

  - This monthly rate is fixed for the initial twelve months.

- This support package will commence after the completion of the Hypercare phase.

  - The client agrees to maintain this support arrangement for a minimum term of six months.

  - After this period, the arrangement will roll over on a monthly basis.

  - The client may terminate the arrangement at any time, with 30 days prior notice.

- The proposed pricing comfortably supports growth of traffic up to 4 times the volumes of the old Motel Mapping system that EAMS is replacing. That is, it will be able to support up to:

  - 8000 total users

  - 800 daily active users

  - 3200 accommodation records

  - The system is designed to scale beyond these initial capacity limits as usage grows. We will monitor usage and discuss with the client well in advance of any infrastructure scaling or cost adjustments (whether usage-driven or due to external factors such as Azure pricing changes).

## Support Response Times

- **Business Hours**: Our standard support hours are Monday to Friday, 9:00 AM to 5:00 PM Melbourne time, excluding public holidays.

- **Response Times**:

  - Critical issues (system down, major functionality broken): Response within 4 business hours

  - High priority issues (significant functionality impaired): Response within 1 business day

  - Normal priority issues (minor bugs, questions): Response within 2 business days

- **After-Hours Support**: While we do not provide guaranteed after-hours support, we will make reasonable efforts to address critical issues outside business hours when possible.

- Issues are typically reported via Trello or email.

  - Trello will be used to track issues.

  - Phone call or text messages are available for urgent issues.

## Monitoring and Operations

- We have set up Azure Application Insights as the primary tool for application and server monitoring.

  - Automatic alerts have been configured to notify us if key server performance metrics (e.g., CPU usage) exceed defined thresholds.

- We will also monitor for other types of issues, such as server errors.

- We will take full responsibility for the health of the application and its underlying infrastructure. This includes:

  - Setting up regular database backups

  - Performing manual backups when necessary

  - Continuously enhancing our recovery plan

  - Providing technical documentation to the client's operations team as a contingency measure

- Except for urgent issues, we usually perform maintenance and fixes during quiet periods (e.g., after hours) to minimise user disruption.


