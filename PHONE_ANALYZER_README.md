# 📱 Phone Performance Analyzer

A comprehensive web-based application that analyzes your mobile phone's hardware performance and battery health based on its age and usage patterns.

## Features

### 📊 Hardware Performance Analysis
- **Overall Performance Score**: Calculates current device performance compared to original specifications
- **Processor Performance**: Evaluates CPU degradation over time
- **Memory Performance**: Assesses RAM efficiency and fragmentation impact
- **Age-based Degradation**: Accounts for natural hardware wear over years of use

### 🔋 Battery Health Analysis
- **Battery Capacity**: Estimates current battery capacity vs. original
- **Charge Cycle Tracking**: Calculates degradation based on estimated charge cycles
- **Usage Pattern Impact**: Adjusts calculations based on light, moderate, or heavy usage
- **Daily Usage Estimates**: Predicts remaining usage time per charge

### 📱 Comprehensive Phone Database
Includes specifications for 70+ popular phone models from major brands:
- **Apple**: iPhone 15 series, iPhone 14 series, iPhone 13, 12, 11, SE, XR
- **Samsung**: Galaxy S24/S23/S22/S21 series, Galaxy A series, Galaxy Z Fold/Flip
- **Google**: Pixel 8, 7, 6, 5 series
- **OnePlus**: OnePlus 12, 11, 10, 9 series, Nord 3
- **Xiaomi**: Xiaomi 14, 13, 12 series, Redmi Note, Poco
- **Huawei**: Mate and P series
- **Oppo**: Find X series, Reno series
- **Vivo**: X series, V series
- **Motorola**: Edge series, Moto G
- **Sony**: Xperia series

## How to Use

1. **Open the App**: Simply open `phone-analyzer.html` in any modern web browser
2. **Select Your Phone**:
   - Choose your phone brand from the dropdown
   - Select your specific model
3. **Enter Phone Age**:
   - Input years (0-10)
   - Input additional months (0-11)
4. **Select Usage Pattern**:
   - **Light**: Basic calls, texts, web browsing
   - **Moderate**: Social media, photos, videos
   - **Heavy**: Gaming, streaming, multitasking
5. **Analyze**: Click "Analyze Performance" button

## Results Breakdown

### Device Information
- Chipset details
- RAM capacity
- Original battery capacity
- Release year
- Current age

### Performance Metrics
Each metric includes:
- Visual progress bar with color coding
- Percentage scores
- Detailed explanations

**Color Coding**:
- 🟢 Green (80-100%): Excellent condition
- 🔵 Blue (60-79%): Good condition
- 🔴 Red (0-59%): Degraded, needs attention

### Recommendations
Personalized suggestions based on your phone's condition:
- Battery replacement advice
- Performance optimization tips
- Security update reminders
- Upgrade recommendations
- Maintenance best practices

## Performance Calculation Methodology

### Hardware Degradation
- **Base Degradation Rate**: 5-12% per year depending on usage
- **Exponential Model**: Degradation accelerates over time
- **Component-Specific**: Different rates for processor vs. memory
- **Usage Multipliers**:
  - Light usage: 0.7x degradation
  - Moderate usage: 1.0x degradation
  - Heavy usage: 1.5x degradation

### Battery Health
- **Cycle-Based**: Assumes 250-500 charge cycles per year
- **Industry Standard**: ~20% capacity loss after 500 cycles
- **Accelerated Degradation**: Faster decline after 500 cycles
- **Usage Impact**: Heavy users see faster battery degradation

### Usage Time Estimation
Based on typical power consumption:
- **Light Usage**: ~200 mAh per hour
- **Moderate Usage**: ~350 mAh per hour
- **Heavy Usage**: ~550 mAh per hour

## Technical Details

- **Pure HTML/CSS/JavaScript**: No external dependencies
- **Responsive Design**: Works on desktop and mobile browsers
- **Client-Side Only**: All calculations performed locally
- **No Data Collection**: Complete privacy, no data sent anywhere
- **Offline Capable**: Works without internet connection after initial load

## Browser Compatibility

Works with all modern browsers:
- Chrome/Edge (v90+)
- Firefox (v88+)
- Safari (v14+)
- Opera (v76+)

## Limitations

- **Estimates Only**: Results are approximations based on industry standards
- **Individual Variance**: Actual performance may vary based on:
  - Specific usage habits
  - Operating system version
  - Number of installed apps
  - Storage capacity used
  - Physical damage or repairs
  - Temperature exposure
  - Charging habits

## Future Enhancements

Potential additions:
- More phone models (older/budget devices)
- Storage performance analysis
- Camera system degradation
- Software update impact
- Custom phone specifications input
- Historical tracking (with local storage)
- Export results as PDF
- Comparison between multiple devices

## Contributing

To add more phone models, update the `phoneDatabase` object with:
```javascript
"Model Name": {
    year: RELEASE_YEAR,
    processor: BENCHMARK_SCORE,
    ram: RAM_IN_GB,
    battery: CAPACITY_IN_MAH,
    chipset: "CHIPSET_NAME"
}
```

## License

This project is part of The Commons initiative - an open-source platform for human flourishing.

## Disclaimer

This tool provides estimates based on industry averages and mathematical models. For accurate battery health readings, use your device's built-in diagnostics or authorized service centers. Performance metrics are approximations and do not replace professional device testing.

---

**Made with ❤️ for The Commons**
