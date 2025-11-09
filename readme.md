# Second Chart Timeframe

![Version](https://img.shields.io/badge/version-1.04-blue)
![MT5](https://img.shields.io/badge/MT5-compatible-orange)
![License](https://img.shields.io/badge/license-MIT-green)

Indikator MetaTrader 5 untuk **candlestick berbasis detik** (1-59 detik). Cocok untuk scalping dan trading frekuensi tinggi.

## Fitur

- Periode detik yang dapat disesuaikan (1-59 detik)
- Update OHLC real-time
- Timer countdown visual
- Tampilan di window terpisah
- Sistem buffer performa tinggi

## Instalasi

1. Copy `SecondTimeframeIndicator.mq5` ke folder `MQL5/Indicators/`
2. Compile di MetaEditor
3. Restart MT5
4. Drag ke chart

## Parameter

| Parameter | Default | Deskripsi |
|-----------|---------|-----------|
| InpSecondPeriod | 5 | Periode dalam detik (1-59) |
| InpCandleColor | DodgerBlue | Warna candle |
| InpCandleWidth | 1 | Lebar garis |
| InpMaxBars | 200 | Maksimal history |
| InpShowInfo | true | Tampilkan info panel |

## Penggunaan

**Scalping (3 detik):**
```mql5
InpSecondPeriod = 3
```

**News Trading (1 detik):**
```mql5
InpSecondPeriod = 1
```

**Konfirmasi Entry (10 detik):**
```mql5
InpSecondPeriod = 10
```

## Kebutuhan Sistem

- MetaTrader 5 Build 3802+
- Market aktif dengan data tick

## Troubleshooting

**Candle tidak muncul?** Pastikan market aktif dan indikator ada di window terpisah.

**Masalah performa?** Kurangi `InpMaxBars` jadi 50-100.

**Timer tidak jalan?** Restart indikator atau MT5.

## Disclaimer

**Hanya untuk tujuan edukasi.** Trading melibatkan risiko. Test di demo terlebih dahulu. Bukan saran finansial.

---

🐛 [Laporkan Issue](https://github.com/msyamsudin/second-precision-tf/issues)