servers down at the moment 
## Healthcare Appointment Booking System

This project is a cloud-hosted web application that allows patients to schedule, cancel, and manage healthcare appointments online. It was built using AWS services including EC2 for the backend API, DynamoDB for storing appointment data, Route 53 for domain management, and Nginx for serving the frontend and acting as a reverse proxy.

The goal was to create a cloud-based application that demonstrates how a real-world booking system can be deployed securely and reliably using AWS infrastructure.

## Features

Frontend website served through Nginx

Node.js + Express backend API running on EC2

DynamoDB table for storing patient and appointment information

Route 53 for domain management with subdomains (app.cloudbookingproject.com and api.cloudbookingproject.com)

HTTPS enabled with Let’s Encrypt SSL certificates

## Challenges

While working on this project, I ran into several issues with Nginx configuration, SSL setup, and connecting the frontend to the backend API through custom domains. These were resolved by carefully configuring Nginx server blocks, setting up DNS records in Route 53, and testing the API endpoints with cURL before integrating the frontend.

## How it works

The frontend is a simple HTML/CSS/JS site with a booking form.

Patients choose a doctor, select a time, and submit their appointment.

The request is sent to the backend API (api.cloudbookingproject.com).

The Node.js server validates the request and stores it in DynamoDB.

A confirmation message is sent back to the frontend to notify the patient.
