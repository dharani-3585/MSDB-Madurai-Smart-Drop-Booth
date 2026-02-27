# MSDB -- Madurai Smart Drop Booth

## An IoT-Enabled Solar-EV Ecosystem for Decentralized Waste Management

------------------------------------------------------------------------

## 1. Executive Summary

MSDB (Madurai Smart Drop Booth) is an IoT-enabled, solar-powered mobile
waste collection ecosystem designed to solve segregation failure and
inefficient waste logistics in Madurai.

Unlike static bins, MSDB is a mobile smart EV van that: - Travels to
dense zones - Accepts only segregated waste - Rewards users with Green
Credits - Sends real-time data to cloud - Operates on 100% solar-neutral
power

------------------------------------------------------------------------

## 2. Problem Statement

### Current Waste Crisis

-   600+ tonnes waste daily
-   70% mixed waste → unusable for recycling
-   No citizen incentive
-   Diesel trucks increase carbon emissions
-   Narrow streets cause inefficiency

### Core Problems

-   Low segregation
-   Overflow bins
-   Logistical inefficiency
-   High carbon footprint

------------------------------------------------------------------------

## 3. Vision & Goals

### Vision

Create India's first Mobile Solar IoT Waste Credit Economy.

### Year 1 Goals (Pilot -- 5 Vans)

-   40% increase in clean plastic recovery
-   10,000 active users
-   15 tonnes/month segregated collection
-   Break-even in 12 months

------------------------------------------------------------------------

## 4. Product Overview

MSDB is a Mobile Smart Waste Buying Station mounted on an EV van.

### Core Features

-   QR-Based Access
-   Smart Hatch System
-   Load Cell Validation (±5g accuracy)
-   AI Camera Verification
-   Green Credit Wallet
-   Solar Powered System
-   Real-Time Admin Dashboard

------------------------------------------------------------------------

## 5. Functional Requirements

### User Flow

1.  Scan QR
2.  Select waste type
3.  Hatch unlocks
4.  Deposit waste
5.  Weight recorded
6.  AI verification
7.  Credits issued

Time per transaction: \< 30 seconds

### Credit Formula

credits = (weight_in_grams / 1000) × rate

------------------------------------------------------------------------

## 6. Technical Architecture

### Hardware Layer

-   Raspberry Pi 4
-   HX711 Load Cells
-   HC-SR04 Ultrasonic Sensors
-   Pi Camera (TensorFlow Lite)
-   4G LTE Module
-   100W Solar Panel + 20Ah LiFePO4 Battery

### Software Layer

-   Python-based edge logic
-   FastAPI backend
-   PostgreSQL database
-   WebSocket notifications
-   JWT authentication

### Sample Payload

``` json
{
  "booth_id": "MDU-VAN-01",
  "user_id": "UID_9876",
  "waste_type": "PLASTIC",
  "weight_gms": 450,
  "timestamp": "2026-02-27T15:00:00Z"
}
```

------------------------------------------------------------------------

## 7. Cost Analysis

  Component                Prototype Cost (₹)   Mass Cost (₹)
  ------------------------ -------------------- ---------------
  Raspberry Pi + Sensors   12,000               7,500
  Solar Kit                8,000                5,500
  Mechanical Hatch         15,000               10,000
  EV Modification          18,000               12,000
  **Total**                **53,000**           **\~35,000**

------------------------------------------------------------------------

## 8. Fraud Prevention

-   AI Vision verification
-   Weight anomaly detection
-   Manual operator alert system
-   Repeat abuse detection

------------------------------------------------------------------------

## 9. Revenue Model

-   Recycler premium buyback
-   CSR sponsorships
-   Government subsidy
-   Carbon credit trading
-   Brand advertising

------------------------------------------------------------------------

## 10. Impact

### Environmental

-   40% increase in high-purity recyclable waste
-   Reduced landfill load

### Economic

-   Self-sustaining waste ecosystem

### Social

-   Gamified cleanliness
-   Youth engagement
-   Green Ambassador programs

------------------------------------------------------------------------

## 11. Roadmap (12 Months)

-   Months 1--2: Prototype
-   Months 3--4: AI training
-   Month 5: Pilot launch
-   Months 6--9: Optimization
-   Months 10--12: Scale to 5 vans

------------------------------------------------------------------------

**MSDB is not just a waste solution --- it is a ClimateTech, GovTech,
and Incentive Economy platform for sustainable cities.**
