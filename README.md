# Crypto Tracker

**Crypto Tracker** is a modern Android application that allows users to monitor real-time cryptocurrency data, explore historical trends, and visualize market changes through dynamic charts — all within a clean, Compose-based UI.


---
## 📸 Screen Shots
<table>
  <tr>
    <td align="center">
      <strong>Splash Screen</strong><br/>
      <img src="https://github.com/user-attachments/assets/0a4c6b67-d993-4278-82dc-59a998a8570e" width="200"/>
    </td>
    <td align="center">
      <strong>Coin Details Portrait</strong><br/>
      <img src="https://github.com/user-attachments/assets/b522a26c-2a0e-438e-b6e5-04eca5f9bfca" width="200"/>
    </td>
    <td align="center">
      <strong>Coin List Portrait</strong><br/>
      <img src="https://github.com/user-attachments/assets/c43b7c0c-6d6f-47dd-9d4b-793a6b7d67c1" width="200"/>
    </td>
    <td align="center">
      <strong>Landscape</strong><br/>
      <img src="https://github.com/user-attachments/assets/8dca3aa9-d5f2-40df-84a6-c9f4b66c1729" width="200"/>
    </td>
  </tr>
</table>

---

## 🧠 Key Concepts

This app is a practical demonstration of:

- Jetpack Compose UI
- Clean MVVM Architecture
- Koin for Dependency Injection
- Ktor for Networking
- Paging3 for pagination
- Room for local caching
- Single Responsibility & SOLID Principles

## 🛠️ Tech Stack

| Tech                    | Usage                         |
|-------------------------|-------------------------------|
| **Kotlin**              | Programming Language          |
| **Jetpack Compose**     | Declarative UI Framework      |
| **MVVM**                | Architecture Pattern          |
| **Koin**                | Dependency Injection          |
| **Ktor**                | Networking Client             |
| **Paging3**             | Pagination                    |
| **Room**                | Local Caching                 |
---
## 🧩 Architecture
<pre>
app
├── core
│   ├── data
│   │   └── networking
│   │       ├── constructUrl.kt
│   │       ├── HttpClientFactory.kt
│   │       ├── responseToResult.kt
│   │       └── safeCall.kt
│   ├── domain
│   │   └── util
│   │       ├── Error.kt
│   │       ├── NetworkError.kt
│   │       └── Result.kt
│   ├── navigation
│   │   └── AdaptiveCoinListDetailPane.kt
│   └── presentaion
│       └── util
│           ├── CoinCodeToResource.kt
│           ├── NetworkErrorToString.kt
│           └── ObserveAsEvents.kt
├── crypto
│   ├── data
│   │   ├── dto
│   │   │   ├── CoinDto.kt
│   │   │   ├── CoinHistoryDto.kt
│   │   │   ├── CoinPriceDto.kt
│   │   │   └── CoinsResponseDto.kt
│   │   ├── mappers
│   │   │   └── coinMapper.kt
│   │   └── RemoteCoinDataSource.kt
│   ├── domain
│   │   ├── CoinDataSource.kt
│   │   ├── Coin.kt
│   │   └── CoinPrice.kt
│   └── presentaion
│       ├── coin_details
│       │   ├── chart
│       │   │   ├── ChartStyle.kt
│       │   │   ├── DataPoint.kt
│       │   │   ├── LineChart.kt
│       │   │   └── ValueLabel.kt
│       │   ├── CoinDetailsScreen.kt
│       │   └── components
│       │       └── InfoCard.kt
│       ├── coin_list
│       │   ├── CoinListAction.kt
│       │   ├── CoinListEvent.kt
│       │   ├── CoinListScreen.kt
│       │   ├── CoinListState.kt
│       │   ├── CoinListViewModel.kt
│       │   └── components
│       │       ├── CoinListItem.kt
│       │       └── PriceChange.kt
│       └── models
│           └── CoinUi.kt
├── CryptoTrackerApp.kt
├── di
│   └── AppModule.kt
├── MainActivity.kt
└── ui
    └── theme
        ├── Color.kt
        ├── Theme.kt
        └── Type.kt
</pre>

---


## 🔧 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/Bilalazam26/CryptoTracker.git
   
2. Open in Android Studio

---

## 🤝 Contributing
Contributions are welcome! Fork the repo, make your changes, and open a pull request.


</pre>

