# Wessel Developer Platform (WDP)

# Naming Conventions

## Purpose

This document defines the standard naming conventions used throughout the Wessel Developer Platform.

Consistent naming improves readability, maintainability, discoverability, automation, and AI-assisted development.

These conventions apply unless a specific technology requires a different standard.

---

# General Principles

Names should be:

- Descriptive
- Consistent
- Predictable
- Easy to search
- Easy to pronounce

Avoid abbreviations unless they are universally understood.

Examples:

Good

UserAuthenticationService

ParkingTransaction

PaymentStatus

Poor

UsrSvc

PTS

Mgr

Util2

---

# Repository Naming

Repositories use lowercase with hyphens.

Format

wdp-<category>-<name>

Examples

wdp-template-framework48

wdp-template-dotnet8

wdp-template-python

wdp-shared-auth

wdp-shared-logging

wdp-cli

Client repositories should use PascalCase.

Examples

ParkingPortal

TicketTracker

ServCraftPortal

---

# Solution Naming

Solution names use PascalCase.

Examples

ParkingPortal.sln

TicketTracker.sln

AuthenticationServer.sln

---

# Project Naming

Projects use PascalCase.

Examples

ParkingPortal.Web

ParkingPortal.API

ParkingPortal.Shared

ParkingPortal.Tests

ParkingPortal.Database

---

# Namespace Naming

Namespaces match project names.

Examples

ParkingPortal.Web.Controllers

ParkingPortal.API.Services

ParkingPortal.Shared.Models

---

# Folder Naming

Folders use PascalCase.

Examples

Controllers

Services

Repositories

Models

Utilities

Configuration

Exceptions

Middleware

Avoid

controller

service

misc

stuff

temp

---

# File Naming

Files match the primary class they contain.

Examples

UserController.cs

PaymentService.cs

JwtAuthentication.cs

---

# Class Naming

Classes use PascalCase.

Classes should be nouns.

Examples

UserService

TicketRepository

PaymentProcessor

ParkingManager

---

# Interface Naming

Interfaces begin with I.

Examples

IUserService

ILogger

IPaymentGateway

---

# Method Naming

Methods use PascalCase.

Methods should describe an action.

Examples

GetUser()

CreateTicket()

CalculateRevenue()

AuthenticateUser()

Avoid

DoStuff()

Run()

Process()

---

# Variable Naming

Local variables use camelCase.

Examples

ticketNumber

userName

totalRevenue

---

# Private Fields

Private fields begin with an underscore.

Examples

_connectionString

_logger

_userRepository

---

# Constants

Constants use PascalCase.

Examples

MaxLoginAttempts

DefaultPageSize

ApiVersion

---

# Enums

Enums use singular PascalCase.

Examples

PaymentStatus

UserRole

GateDirection

---

# SQL Database Tables

Tables use PascalCase and plural nouns.

Examples

Users

Transactions

Payments

ParkingSessions

---

# SQL Primary Keys

Use

Id

or

<TableName>Id

Examples

Id

UserId

TransactionId

---

# SQL Stored Procedures

Stored procedures begin with

sp_

Examples

sp_GetUsers

sp_CreatePayment

sp_CloseParkingSession

---

# SQL Views

Views begin with

vw_

Examples

vw_CurrentSessions

vw_DailyRevenue

---

# SQL Functions

Functions begin with 

fn_

Examples

fn_CalculatePArkingFee

fn_CreateAccount

fn_ClearPayment

---

# SQL Triggers

Triggers begin with 

trg_

Examples

trg_Payment_Insert

trg_Account_Create

trg_User_Delete

---

# SQL Indexes

Indexes begin with 

IX_

Examples

IX_Users_Email

---

# SQL Foreign Keys

Foreign Keys begin with

FK_

Examples

FK_Payments_Users

FK_Report_Users

---

# API Routes

Routes use lowercase.

Examples

api/users

api/payments

api/reports

Avoid PascalCase.

---

# Git Branches

Feature work

feature/login

feature/payment-report

feature/jwt-authentication

Bug fixes

bugfix/login-timeout

bugfix/payment-rounding

Hotfixes

hotfix/security-patch

Documentation

docs/naming-conventions

Refactoring

refactor/authentication

---

# Commit Messages

Follow Conventional Commits.

Examples

feat:

fix:

docs:

refactor:

test:

style:

perf:

ci:

build:

Examples

feat(auth): implement JWT authentication

fix(api): correct login validation

docs(platform): add architecture documentation

---

# Environment Variables

Use uppercase with underscores.

Examples

JWT_SECRET

DATABASE_CONNECTION

API_KEY

---

# Configuration Files

Use standard platform names.

Examples

appsettings.json

launch.json

settings.json

---

# Documentation

Documentation files use PascalCase.

Examples

Architecture.md

Vision.md

Roadmap.md

NamingConventions.md

---

# Engineering Principle

Good naming reduces the need for comments.

Code should explain itself through consistent and descriptive naming.