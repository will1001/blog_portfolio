---
title: "How to deploy Next.js to Vercel with CI/CD Integration"
date: 2023-05-13T13:06:38+08:00
description: ""
author: "wili"
tags: ["Next Js", "Vercel", "CI/CD"]
theme: "light"
featured: true
cover: "https://miro.medium.com/v2/resize:fit:1100/format:webp/1*1wlhJyfUNUox4Lj7eXO51w.png"
---

# 1. CI/CD

CI/CD is a set of practices and tools that automate the building, testing, and deployment of software applications. It aims to make the development and deployment process faster, more reliable, and less error-prone. By automatically building, testing, and deploying code changes, CI/CD helps developers catch and fix errors early in the development cycle, reduce the cost of development, and improve the quality of the final product. It also ensures that software is always in a deployable state, which makes it easier to release new features to customers more frequently.

# 2. NEXT JS

Next.js is an open-source web development framework that allows developers to build server-side rendered web applications with ease. It provides powerful tools and features such as server-side rendering, easy client-side routing, and support for serverless functions. Next.js is highly customizable and flexible, making it a popular choice for developers and companies to build web applications of any size and complexity, from small marketing sites to large-scale e-commerce platforms.

# 3. VERCEL

Vercel is a cloud platform for building, deploying, and scaling serverless web applications and static websites. It is designed to be easy to use and provides a seamless experience for developers to build and deploy their applications quickly. Vercel supports many popular frameworks and libraries, including Next.js, React, Angular, Vue.js, and more. One of the key benefits of Vercel is its automatic scaling capabilities, which allows applications to handle any amount of traffic without manual intervention. It also provides features such as real-time collaboration, continuous deployment, and custom domains to make the development and deployment process more efficient and streamlined.

# 4. NEXT JS INSTALLATION

First, install Next.js. Here, I’m using automatic installation using `npx`.

![Automatic installation next js command](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*XJEnCrKSqzyZcV21dbHrbQ.png)

Configuring Next.js, it’s up to your needs, or you can follow my configuration.

![](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*Qy5D-k9nwhS662yEdFFpFQ.png)

After successfully opening the project folder using a code editor, in this article, I am using Visual Studio Code (VSCode).

After that, open the terminal in VSCode and then type `npm run dev`.

![](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*Qy5D-k9nwhS662yEdFFpFQ.png)

Then, open [http://localhost:3000/](http://localhost:3000/) in your web browser.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*ZgnasuuB_mRAWw2vstZ73w.png)

# 5. SETUP GIT AND REPOSITORY ON GITHUB

create new repository

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*kSikKqXC0e7-4rEa3zPGuA.png)

Initialize and add remote Git repository in VSCode

![](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*D98yPdaR5osdhSwl10jCTw.png)

If successful, your GitHub repository will look like the image below

![](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*9KPPdGsbXfzcyEnTYIVnPg.png)

# 6. SETUP VERCEL

First, sign up for an account on [https://vercel.com/](https://vercel.com/).

After signing up, open the “Overview” tab in your Vercel account.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*2GXTSi9wNwSl8xqGAr-0xQ.png)

Then, add a new project.

![](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*9DASpMkYyDjI5b-wQy-Z0Q.png)

Next, import the repository that you have created before.

Use the default configuration and click the “Deploy” button.

![](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*LaCQipmEAEDnW-KiJx1OJw.png)

Wait for the deployment process to finish. If it is done, it will look like this.

![](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*PwBbKN15IUJ1qEK_2m_rXA.png)

![](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*hzfoVbKe0T3foJmcpEckhg.png)

click visit and your next js website has been deployed!.

![](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*McELskaI5y_uFqaZk8qAGA.png)

To test CI/CD, make changes to the `pages.tsx` file, and then commit and push it to your GitHub repository.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*J9Zqsz-8rZuez2EbdnIkxA.png)

Wait until your GitHub repository has a green checkmark.

![](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*bCIy05-4iyGe4O8EYlA0PQ.png)

Then, check your Vercel link again and refresh the page.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*kSikKqXC0e7-4rEa3zPGuA.png)
