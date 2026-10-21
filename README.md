# Room Products

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white)
![Room](https://img.shields.io/badge/Room-2.6-3DDC84?style=flat-square&logo=android&logoColor=white)

A product list cached in **Room** with live search. The search field is turned into a `Flow` that is **debounced** (300 ms) and switched with **`flatMapLatest`**, so only the latest query hits the database and stale results are dropped.

> Lab #5 · Mobile Application Development course. Ukrainian version: [README.uk.md](README.uk.md)

## Features

- Products stored in Room and observed as `Flow`
- Search by name or category with a SQL `LIKE` query
- Debounced input: no query per keystroke
- Cache refresh that replaces the stored list

## Tech stack

Kotlin · Jetpack Compose · Material 3 · Room · Coroutines & Flow · ViewModel

## Run locally

Open in Android Studio (Iguana or newer), let Gradle sync, run on API 26+.
