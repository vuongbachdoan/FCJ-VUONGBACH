---
date:
  created: 2023-12-30
comments: true
categories:
  - Datadog
  - Monitoring
theme:
  features:
    - toc.integrate
---

# Monitoring with Datadog

![AWS Cloud Club Logo](assets/images/datadog/1.png)

<!-- material/tags { toc: true } -->

## Introduction
- **Goal:** Monitoring with Datadog
- **Duration:** 15 Jul 2024 - 19 Jul 2024
- **Training Type:** Offline / Online, Self-paced
- **Target Audience:** Individuals interested in using Datadog for system monitoring
- **Complexity:** Beginner
- **Prerequisites:** None

<!-- more -->

---

## Overview About Monitoring

Datadog excels at collecting a wide range of metrics from various sources, including systems, applications, and custom integrations.

### What Will We Monitor?

#### 1. WORK METRICS
Work metrics indicate the top-level health of your system by measuring its useful output. These metrics are invaluable for surfacing real, often user-facing issues. They include:
- **Throughput:** The amount of work the system is doing per unit time.
- **Success Metrics:** The percentage of work executed successfully.
- **Error Metrics:** The rate of errors per unit time or per unit of work.
- **Performance Metrics:** Efficiency measurements, such as latency.

#### 2. RESOURCE METRICS
Resource metrics provide insights into the components of your software infrastructure. Key areas to cover:
- **Utilization:** Percentage of time the resource is busy.
- **Saturation:** Measure of the amount of requested work that cannot yet be serviced.
- **Errors:** Internal errors not observable in the work output.
- **Availability:** Percentage of time the resource responded to requests.

#### 3. EVENTS
Events provide crucial context for understanding system behavior changes. Examples include:
- **Code Changes:** Releases, builds, and build failures.
- **Alerts:** Notifications from monitoring systems or third-party tools.
- **Scaling Events:** Adding or subtracting hosts or containers.

### Introducing Graphs

#### 1. TIMESERIES
Line graphs visualize metric data, useful for:
- Spotting outliers, tracking single metrics, or spotting individual deviations.
- Stacked Area Graphs show sum and part contributions at a glance.

#### 2. SUMMARY GRAPHS
- **Single-Value Summaries:** Highlight key metrics visibly.
- **Toplists:** Rank segments by metric values, useful for spotting outliers.
- **Change Graphs:** Compare current metric values against past values.
- **Host Maps:** Visualize resource utilization and identify issues.
- **Distributions:** Histogram of metric values across infrastructure.

---

## Demo

### 🖥️ Demo - Monitoring EC2 Server
1. **Install the Agent:** Follow Datadog's documentation for installation instructions.
2. **Configure the Agent:** Specify metrics to collect and their frequency.
3. **Datadog Monitoring:** Access detailed metrics via Datadog dashboards.

### 🐳 Demo - Monitoring Kubernetes Cluster
1. **Install the Datadog Agent:** Deploy Cluster and Node Agents in your cluster.
2. **Leverage kube-state-metrics:** Gain insights into Kubernetes object health.
3. **Enable Autodiscovery:** Automatically detect and collect metrics from cluster components.

### 🚀 Demo - Monitoring Lambda Function
1. **Create the Datadog Lambda Layer:** Add the Datadog Lambda library to your function.
2. **Add the Layer to your Lambda Function:** Configure in AWS Management Console.
3. **Datadog Integration and Monitoring:** Ensure Datadog access and start monitoring.

## 🏷️ Custom Metrics and Tags
Custom metrics and tagging allow for extended monitoring capabilities:

- **Defining and Sending Custom Metrics:** Tailor Datadog monitoring to specific needs.

- **Using Tags:** Effectively categorize and filter metrics.

- **Creating Tailored Dashboards and Alerts:** Utilize custom metrics and tags for personalized monitoring setups.
