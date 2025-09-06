# Heavy-Tailed Distributions in Behavioral Asset Pricing

A comprehensive empirical and theoretical framework analyzing the superiority of heavy-tailed distributions over normal assumptions in behavioral asset pricing models.

## Key Findings

- **Universal normality rejection**: 100% of 86 assets across 25 categories reject normal distribution assumptions
- **Student's t dominance**: Achieves best-model status in 88.4% of cases using AIC criteria  
- **Risk underestimation**: Normal models systematically underestimate 99% VaR by 19.7% on average
- **Mathematical consistency**: Framework maintains infinite divisibility properties essential for dynamic pricing

## Dataset

- **86 assets** across 25 categories (US equities, international, bonds, commodities, REITs, sectors)
- **432,752 observations** spanning January 2004 to December 2024
- **20+ years** of data covering multiple economic cycles

## Methodology

- **Statistical testing**: Shapiro-Wilk, Jarque-Bera, Anderson-Darling, Kolmogorov-Smirnov
- **Distribution fitting**: Maximum likelihood estimation with AIC/BIC model selection
- **Risk analysis**: VaR backtesting and Expected Shortfall validation
- **Theoretical framework**: Random agent models with probability weighting integration

## Usage

```bash
# Clone repository
git clone https://github.com/akashdeepo/Heavy-Tailed-Distributions-in-Behavioral-Asset-Pricing
cd Heavy-Tailed-Distributions-in-Behavioral-Asset-Pricing

# Install dependencies
pip install numpy pandas scipy matplotlib seaborn yfinance

# Run analysis
jupyter notebook Enhanced_Behavioral_Asset_Pricing.ipynb
```

## Requirements

- Python 3.12+
- numpy 2.0.2
- pandas 2.2.2  
- scipy 1.16.1
- matplotlib 3.10.0
- seaborn 0.13.2
- yfinance 0.2.65

## Project Structure

```
├── Enhanced_Behavioral_Asset_Pricing.ipynb    # Main analysis notebook
├── figure1_empirical_evidence.png             # Generated figures
├── figure2_model_performance.png
├── table_descriptive_statistics.csv           # Summary tables
├── table_distribution_comparison.csv
├── research_summary.txt                       # Key findings
└── README.md
```

## Results

### Distribution Performance
| Distribution | Avg AIC | Best Model % |
|-------------|---------|--------------|
| Normal      | -26,250 | 0.0%         |
| Student's t | -27,816 | 88.4%        |
| Laplace     | -27,284 | 11.6%        |

### Risk Measurement Accuracy
- **Normal VaR Error**: 19.7% underestimation
- **Student's t VaR Error**: 3.2% average error
- **Regulatory Impact**: Significant for Basel III compliance

## Theoretical Contributions

1. **Random agent models** addressing finite mixture limitations
2. **Infinite divisibility preservation** ensuring mathematical consistency
3. **FTAP compatibility** for arbitrage-free dynamic pricing
4. **Behavioral integration** through probability weighting functions

## Applications

- **Risk Management**: More accurate tail risk measurement
- **Portfolio Optimization**: Better risk-return estimation  
- **Derivative Pricing**: Improved tail probability modeling
- **Regulatory Compliance**: Enhanced Basel III/MiFID II validation

## Citation

```bibtex
@article{deep2024heavy,
  title={Heavy-Tailed Distributions in Behavioral Asset Pricing: A Comprehensive Framework for Dynamic Markets},
  author={Deep, Akash and Rachev, Svetlozar T. and Fabozzi, Frank J.},
  journal={Working Paper},
  year={2024}
}
```

## License

MIT License - see LICENSE file for details

## Authors

- **Akash Deep** - Texas Tech University (akash.deep@ttu.edu)
- **Svetlozar T. Rachev** - Texas Tech University  
- **Frank J. Fabozzi** - Johns Hopkins University

---

*This research provides the first mathematically consistent behavioral asset pricing framework that maintains empirical realism while satisfying arbitrage-free conditions essential for institutional applications.*
