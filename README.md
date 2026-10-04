# n8n Reporting Agent

**Generates periodic business reports with trend summaries and delivers them by email (SMTP) or Slack on a cron schedule. Data sources are sample data in this version.**

> **This is a proprietary project. Source code is private. This page showcases the system's architecture and results.**

**Case study page:** [https://jryahia.github.io/showcase-n8n-reporting-agent/](https://jryahia.github.io/showcase-n8n-reporting-agent/)

![n8n Reporting Agent](assets/00-dashboard.png)

## Problem it solves

Weekly reporting usually means someone copying numbers from several tools into a document. This agent collects the data, writes the summary and delivers it on a cron schedule. It is built as the webhook backend for a n8n scenario: the automation platform handles triggers, and this service holds the logic and data.

## Architecture

![Architecture](assets/architecture.svg)

1. Sources are synced on demand or on a schedule.
2. A report is generated with trend summaries for the period.
3. The report is delivered by email or Slack.
4. Each delivery attempt is logged.

## Key features

- On-demand and scheduled reports
- Multi-source data collection
- Email and Slack delivery with logs
- Cron schedules managed via API
- Report history

## Tech stack

![Python](https://img.shields.io/badge/Python-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![FastAPI](https://img.shields.io/badge/FastAPI-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![Webhooks](https://img.shields.io/badge/Webhooks-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![Slack Webhooks](https://img.shields.io/badge/Slack%20Webhooks-161b22?style=for-the-badge&labelColor=161b22&color=161b22) ![SMTP](https://img.shields.io/badge/SMTP-161b22?style=for-the-badge&labelColor=161b22&color=161b22)

## What it does in practice

- Prototype stage: report generation, scheduling and delivery are built; CRM, analytics and revenue collectors return sample data.

## Screenshots

**Reports, data sources and schedules**

![Reports, data sources and schedules](assets/00-dashboard.png)

**API surface: reports, sources, schedules, delivery**

![API surface: reports, sources, schedules, delivery](assets/10-api.png)

---

Built by [Yahya Jarray](https://github.com/jryahia). Interested in a similar system? [Get in touch](mailto:yahiajarray43@gmail.com).

This repository contains no source code. It is a case study for a proprietary project. © Yahya Jarray.
