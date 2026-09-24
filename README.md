<div align="center">

<h1>Moodle M-Pesa Plugin</h1>

<p>
<strong>Moodle M-Pesa enrolment plugin using the Safaricom Daraja API</strong>
</p>

<p>
Accept M-Pesa payments and automatically enrol students into Moodle courses, classes, lessons, or tutorials after successful payment.
</p>

<p>
<a href="#installation">Installation</a> •
<a href="#configuration">Configuration</a> •
<a href="#how-it-works">How It Works</a> •
<a href="#frequently-asked-questions">FAQs</a> •
<a href="#support">Support</a>
</p>

<br>

<a href="https://wa.me/254706745202">
<img src="https://img.shields.io/badge/WhatsApp-Contact%20Me-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="Contact on WhatsApp">
</a>

</div>

---

## Overview

The **Moodle M-Pesa plugin** integrates **Moodle** with the **Safaricom M-Pesa Daraja API** to provide an automated payment and enrolment workflow.

Your Moodle website users, including **students, trainees, and learners**, can enrol into your different classes or lessons by paying with M-Pesa mobile money.

The payment process is designed to be simple:

1. The student selects **M-Pesa** from the available Moodle payment methods.
2. The student enters their **M-Pesa phone number (MSISDN)**.
3. An **M-Pesa STK Push** prompt appears on the student's phone.
4. The student enters their **M-Pesa PIN** to authorize the payment.
5. The payment is processed through the **Daraja API**.
6. After successful payment, the system automatically **enrols the student into the selected Moodle course, class, lesson, or tutorial**.

This makes it possible to sell access to Moodle-based learning without requiring students to make a manual payment and then wait for an administrator to enrol them.

---

<a id="how-it-works"></a>

## How It Works

```text
Student
   │
   ▼
Selects Moodle Course
   │
   ▼
Selects M-Pesa Payment
   │
   ▼
Enters M-Pesa Phone Number
   │
   ▼
M-Pesa STK Push
   │
   ▼
Student Enters M-Pesa PIN
   │
   ▼
Daraja API Processes Payment
   │
   ▼
Successful Payment
   │
   ▼
Automatic Moodle Enrolment
   │
   ▼
Student Accesses Course
```

---

## Features

<ul>
<li>M-Pesa payment integration for Moodle</li>
<li>Safaricom Daraja API integration</li>
<li>M-Pesa STK Push payment workflow</li>
<li>Students can enter their M-Pesa phone number during enrolment</li>
<li>Automatic enrolment after successful payment</li>
<li>Suitable for paid Moodle courses</li>
<li>Suitable for classes, lessons, tutorials, and training programs</li>
<li>Reduces manual payment verification and enrolment</li>
<li>Designed for Moodle websites accepting M-Pesa mobile money</li>
</ul>

---

## Payment and Enrolment Flow

When a learner wants to purchase access to a Moodle course, they can select **M-Pesa** from the enabled payment methods.

The learner enters their M-Pesa **MSISDN/mobile phone number**.

An M-Pesa **STK Push** prompt is then sent to the learner's phone.

The learner enters their M-Pesa PIN to authorize the transaction.

After the payment is successfully processed, the plugin handles the enrolment process so that the learner can be enrolled into the specific Moodle course, class, lesson, or tutorial.

---

## Requirements

Before using the plugin, you should have:

<ul>
<li>A working Moodle website</li>
<li>A Moodle course configured for paid enrolment</li>
<li>An M-Pesa account suitable for receiving payments</li>
<li>Access to the Safaricom <strong>Daraja API</strong></li>
<li>The required Daraja API credentials</li>
<li>A Moodle installation where enrolment/payment plugins can be installed</li>
</ul>

The exact Daraja configuration and credentials required may depend on your M-Pesa account and deployment environment.

---

## M-Pesa Daraja API

This plugin uses the **Safaricom Daraja API** to communicate with M-Pesa.

The Daraja integration allows the Moodle website to initiate an M-Pesa payment request and process the resulting payment response.

You should obtain and configure the appropriate Daraja API credentials before using the plugin for live transactions.

For Daraja API documentation and account setup, refer to Safaricom's official Daraja documentation.

---

<a id="installation"></a>

## Installation

Download or clone this repository into your Moodle installation in the appropriate enrolment plugin directory.

For example:

```text
moodle/
└── enrol/
    └── your_plugin_directory/
```

After copying the plugin into Moodle:

<ol>
<li>Log in to Moodle as an administrator.</li>
<li>Open the Moodle administration area.</li>
<li>Complete the plugin installation/upgrade process.</li>
<li>Configure the M-Pesa/Daraja API settings.</li>
<li>Enable the M-Pesa enrolment/payment method.</li>
<li>Configure your Moodle course for paid enrolment.</li>
<li>Test the payment process before using it for live transactions.</li>
</ol>

<blockquote>
The exact installation directory and configuration options may depend on the plugin version and your Moodle installation.
</blockquote>

---

<a id="configuration"></a>

## Configuration

After installation, configure the plugin with the required M-Pesa Daraja API settings.

You will generally need to configure the credentials and payment settings required by your Daraja environment.

After configuration, make sure that:

<ul>
<li>M-Pesa is enabled as a payment/enrolment method.</li>
<li>The relevant Moodle course has a price configured.</li>
<li>The M-Pesa payment settings are correct.</li>
<li>Your Daraja API credentials are valid.</li>
<li>Your callback/response configuration is correctly configured where required.</li>
<li>You have tested the complete payment and enrolment workflow.</li>
</ul>

---

## Using M-Pesa for Moodle Courses

Once configured, students can use the plugin during the Moodle enrolment process.

For example, a training website could offer:

```text
Course: Introduction to Computer Programming
Price: KES 5,000

Payment Method:
✓ M-Pesa

Student enters:
+254XXXXXXXXX

        ↓

M-Pesa STK Push

        ↓

Student enters M-Pesa PIN

        ↓

Payment successful

        ↓

Student automatically enrolled
```

The same concept can be used for different types of Moodle learning products.

Examples include:

<ul>
<li>Online courses</li>
<li>Training programs</li>
<li>Professional courses</li>
<li>Classes</li>
<li>Lessons</li>
<li>Tutorials</li>
<li>Workshops</li>
<li>Educational programs</li>
</ul>

---

## Automatic Enrolment

One of the main purposes of the plugin is to connect the payment process with Moodle enrolment.

Instead of requiring an administrator to manually check whether a student has paid and then enrol that student, the successful M-Pesa payment can trigger the Moodle enrolment process.

This provides a more automated workflow for Moodle websites selling paid learning content.

---

<a id="frequently-asked-questions"></a>

# Frequently Asked Questions

<h2>FAQs 1</h2>

<details>
<summary><strong>How do I install the Moodle M-Pesa plugin?</strong></summary>

<p>
Download or clone the plugin into your Moodle installation, place it in the appropriate enrolment plugin directory, and complete the installation and configuration from the Moodle administration interface.
</p>

<p>
You will need to configure the M-Pesa Daraja API credentials and payment settings before accepting live payments.
</p>

</details>

<br>

<details>
<summary><strong>How do I configure M-Pesa payments in Moodle?</strong></summary>

<p>
After installing the plugin, configure your M-Pesa Daraja API credentials and the required payment settings in Moodle.
</p>

<p>
Once configured, enable M-Pesa as an available payment method so students can select it when enrolling into a course.
</p>

</details>

<br>

<details>
<summary><strong>How can students pay for a Moodle course using M-Pesa?</strong></summary>

<p>
Students select M-Pesa as their payment method, enter their M-Pesa phone number (MSISDN), and initiate the payment.
</p>

<p>
An M-Pesa STK Push prompt appears on their phone, where they enter their M-Pesa PIN to authorize the transaction.
</p>

</details>

<br>

<details>
<summary><strong>Does the plugin automatically enrol students after payment?</strong></summary>

<p>
Yes. After a successful M-Pesa payment, the plugin can automatically enrol the student into the selected Moodle course, class, lesson, or tutorial.
</p>

</details>

<br>

<details>
<summary><strong>How can I get help configuring the Moodle M-Pesa plugin?</strong></summary>

<p>
For installation, configuration, M-Pesa Daraja API integration, or consultation, contact me on WhatsApp:
</p>

<p>
<strong>+254 706 745 202</strong>
</p>

</details>

<br>

<details>
<summary><strong>How can I get the Pro version of the Moodle M-Pesa plugin?</strong></summary>

<p>
If you need the Pro version or additional functionality beyond the available implementation, contact me on WhatsApp:
</p>

<p>
<strong>+254 706 745 202</strong>
</p>

<p>
You can discuss the Pro version and your requirements directly.
</p>

</details>

<br>

<details>
<summary><strong>How can I get M-Pesa Daraja API integration for my Moodle website?</strong></summary>

<p>
This plugin provides an M-Pesa payment integration for Moodle using the Safaricom Daraja API.
</p>

<p>
If you need help integrating or configuring the plugin for your Moodle website, contact me on WhatsApp:
</p>

<p>
<strong>+254 706 745 202</strong>
</p>

</details>

---

<h2>FAQs 2</h2>

<details>
<summary><strong>Is the Moodle M-Pesa plugin suitable for online courses?</strong></summary>

<p>
Yes. The plugin is designed for Moodle websites where students, trainees, or learners need to pay for courses, classes, lessons, or tutorials before being enrolled.
</p>

</details>

<br>

<details>
<summary><strong>What does the Moodle M-Pesa plugin do?</strong></summary>

<p>
The plugin connects Moodle enrolment payments with M-Pesa through the Daraja API.
</p>

<p>
It allows a learner to select M-Pesa, enter their phone number, authorize an STK Push payment, and be automatically enrolled after successful payment.
</p>

</details>

<br>

<details>
<summary><strong>Can I use M-Pesa to sell Moodle courses?</strong></summary>

<p>
Yes. A Moodle website can use the plugin to accept M-Pesa payments for courses or other paid learning activities and automatically enrol learners after successful payment.
</p>

</details>

<br>

<details>
<summary><strong>Does the plugin support M-Pesa STK Push?</strong></summary>

<p>
Yes. The payment process uses an M-Pesa STK Push prompt, allowing the learner to authorize the payment directly from their mobile phone using their M-Pesa PIN.
</p>

</details>

<br>

<details>
<summary><strong>Do students need to manually enrol after paying?</strong></summary>

<p>
No. After successful payment, the plugin can automatically enrol the student into the corresponding Moodle course, class, lesson, or tutorial.
</p>

</details>

<br>

<details>
<summary><strong>Is this Moodle M-Pesa plugin free?</strong></summary>

<p>
The availability and features of the free implementation and Pro version may differ.
</p>

<p>
If you require the Pro version or additional functionality, contact me on WhatsApp at <strong>+254 706 745 202</strong> for details.
</p>

</details>

<br>

<details>
<summary><strong>Who is this Moodle M-Pesa plugin for?</strong></summary>

<p>
The plugin can be useful for:
</p>

<ul>
<li>Moodle administrators</li>
<li>Schools</li>
<li>Colleges</li>
<li>Universities</li>
<li>Training centres</li>
<li>Tutors</li>
<li>Online course providers</li>
<li>Professional training organizations</li>
<li>Businesses providing online training</li>
</ul>

</details>

<br>

<details>
<summary><strong>Can you help me integrate M-Pesa with my Moodle website?</strong></summary>

<p>
Yes. Installation, configuration, integration, customization, and consultation can be discussed via WhatsApp.
</p>

<p>
<strong>WhatsApp: +254 706 745 202</strong>
</p>

</details>

<br>

<details>
<summary><strong>Can I purchase or request the Pro version?</strong></summary>

<p>
Yes. For the Pro version, commercial requirements, customization, installation assistance, or consultation, contact:
</p>

<p>
<strong>+254 706 745 202</strong>
</p>

</details>

---

<h2>M-Pesa Moodle Integration FAQs</h2>

<details>
<summary><strong>What is required to connect Moodle to M-Pesa?</strong></summary>

<p>
The integration uses the Safaricom Daraja API.
</p>

<p>
You will need the appropriate Daraja API credentials and a suitably configured Moodle installation.
</p>

</details>

<br>

<details>
<summary><strong>Does the plugin use the Safaricom Daraja API?</strong></summary>

<p>
Yes. The plugin implementation is designed to integrate Moodle enrolment payments with M-Pesa through the Daraja API.
</p>

</details>

<br>

<details>
<summary><strong>Can M-Pesa payments automatically unlock a Moodle course?</strong></summary>

<p>
Yes. Once the payment is successfully processed, the plugin can automatically enrol the learner into the corresponding Moodle course, allowing access according to Moodle's enrolment configuration.
</p>

</details>

<br>

<details>
<summary><strong>Can I use the plugin for paid classes and tutorials?</strong></summary>

<p>
Yes. The plugin can be used for Moodle courses, classes, lessons, tutorials, and other learning activities configured for paid enrolment.
</p>

</details>

<br>

<details>
<summary><strong>Where can I get the Moodle M-Pesa plugin?</strong></summary>

<p>
The source code and implementation are available through this GitHub repository.
</p>

<p>
For the Pro version, installation assistance, customization, or consultation, contact <strong>+254 706 745 202</strong> on WhatsApp.
</p>

</details>

---

# Pro Version and Consultation

<div align="center">

<h2>Need the Pro Version or Integration Help?</h2>

<p>
If you need additional functionality, customization, installation assistance, or the <strong>Pro version</strong> of the Moodle M-Pesa plugin, get in touch.
</p>

<br>

<a href="https://wa.me/254706745202">
<img src="https://img.shields.io/badge/WhatsApp-+254%20706%20745%20202-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="Contact on WhatsApp">
</a>

<br><br>

<strong>WhatsApp: +254 706 745 202</strong>

</div>

You can contact me for:

<ul>
<li>Pro version</li>
<li>Installation</li>
<li>Configuration</li>
<li>M-Pesa Daraja API integration</li>
<li>Moodle integration</li>
<li>Customization</li>
<li>Technical consultation</li>
</ul>

---

# Why Use M-Pesa for Moodle?

For Moodle websites serving learners who use M-Pesa, integrating mobile money payments can simplify the process of purchasing course access.

Instead of requiring learners to:

```text
Make payment
     ↓
Send payment confirmation
     ↓
Wait for administrator
     ↓
Administrator verifies payment
     ↓
Administrator enrols student
```

the plugin provides an automated payment-to-enrolment workflow:

```text
Select Course
     ↓
Select M-Pesa
     ↓
Enter Phone Number
     ↓
STK Push
     ↓
Enter M-Pesa PIN
     ↓
Payment
     ↓
Automatic Enrolment
```

---

# Intended Use

This plugin is intended for Moodle websites that want to integrate M-Pesa payments with Moodle enrolment.

Before using the plugin for production payments, administrators should properly configure and test their Moodle installation, M-Pesa account, Daraja API credentials, payment callbacks, and enrolment settings.

---

<a id="support"></a>

# Support

<div align="center">

<p>
For enquiries, consultation, installation assistance, customization, or the Pro version:
</p>

<a href="https://wa.me/254706745202">
<img src="https://img.shields.io/badge/WhatsApp-Contact%20+254706745202-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp Support">
</a>

<p>
<strong>+254 706 745 202</strong>
</p>

</div>

---

# Keywords

Moodle M-Pesa plugin, Moodle M-Pesa integration, M-Pesa Moodle, Moodle Daraja API, Moodle payment plugin, Moodle enrolment plugin, M-Pesa STK Push Moodle, Safaricom Daraja Moodle, Moodle course payment, Moodle M-Pesa payment, sell Moodle courses with M-Pesa, Moodle automatic enrolment, M-Pesa online course payment, Moodle mobile money payment.

---

# License

See the repository license and accompanying source files for licensing information.
