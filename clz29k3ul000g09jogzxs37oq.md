---
title: "My observations on React Native as a web developer"
seoTitle: "My observations on React Native as a web developer"
seoDescription: "As a seasoned web developer, I never had the need to build an actual mobile application, until recently I thought of giving it a try to understand how..."
datePublished: Fri Jul 26 2024 05:30:14 GMT+0000 (Coordinated Universal Time)
cuid: clz29k3ul000g09jogzxs37oq
slug: my-observations-on-react-native-as-a-web-developer
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1723879319458/34930c44-195c-4db5-b0eb-a66d1f7523d9.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1723879323853/9486a5f5-9d35-48b5-9947-c01aff6332fd.png
tags: react-native, tech

---

As a seasoned web developer, I never had the need to build an actual mobile application, until recently I thought of giving it a try to understand how native applications work and interact with the devices.

The truth is, I did try to create some applications a long time ago using some poor-quality no-code tools.

## Getting started

Thanks to Expo, building React Native mobile applications has never been easier. To me, it felt very similar to the architecture of Next.js in terms of development experience.

Expo has really clear and concise documentation with a few commands to get started with it, you can also choose any base template for your app using the command line interface as well.

## My learning motive

The main reason I tried app development was to understand how it works, including the flow of execution, building, and deployment process on the Play Store and App Store.

1. **Understanding how bundling works:** The bundling process was initially confusing. I had to learn how Metro bundler works with React Native and how it optimizes the app for performance.
    
2. **Remote configs:** The first time I encountered the concept of remote config, I was amazed by its capabilities. You can have dynamic content and application flow based on the country, audience type, demographic, and more.
    
3. **Native features:** I was amazed by how apps can launch their own widgets to be added to the home screen or interactable widgets on iOS dynamic islands. I really wanted to try bridging them via React Native myself. Although I haven't implemented it yet, I'm eager to dive into it soon.
    
4. **Version updates vs in-app updates:** Differences between updating the app on the app stores versus pushing updates directly to users make me think about the architecture that applications use.
    

# Obstacles I faced

Undoubtedly, I took on quite a complex task for a beginner like me as my first project in app development.

The major obstacles I encountered were:

1. **Build generation:** A significant obstacle I faced was the realization that building for Android and iOS requires a complete different approaches, even with the cross-platform capabilities of React Native. there were many platform-specific considerations that needed to be addressed.
    
2. **High level designing:** Though the stack was mostly similar to React, things were used in such a structured way that it gave me a broader perspective on how I would implement my next web development project in a different manner.
    
3. **Environment variable management:** Funnily enough, I struggled to get environment variables to work in my React Native application. I tried the react-native-dotenv package, but it didn't work at all. Many developers suggested using react-native-config, so I gave it a try, but that didn't work for me either.
    
    The simplest solution I came up with was to export the variables from a simple JavaScript file as an object.
    
4. **Firebase version conflicts:** I was trying to use Firebase auth with persistent storage. As per documentation the widely used method was deprecated and the new documentation was not updated with the latest changes. Thus I had to find a way out and this single problem statement cost me around 4-5 hours only.