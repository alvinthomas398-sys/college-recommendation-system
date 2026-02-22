# College Recommendation System 🎓

A comprehensive Python-based college recommendation system that helps students find the best colleges in India based on their preferences and criteria.

## Overview

This project implements an intelligent college recommendation system that filters and recommends Indian colleges based on multiple criteria such as:
- College ranking
- Placement rates
- Location/State
- College type (Government/Private)
- Annual fees/budget
- Multiple criteria combination

## Features ✨

- **Interactive Menu Interface**: User-friendly command-line interface
- **Multiple Recommendation Filters**:
  - By ranking
  - By placement rate
  - By state location
  - By college type
  - By budget (annual fees)
  - Multi-criteria recommendations

- **Data Management**:
  - Load college data from CSV
  - Search colleges by name
  - View statistics and insights

- **Visualizations**:
  - Ranking vs Placement scatter plot
  - College type distribution
  - Top colleges ranking
  - Placement rate by college type
  - State distribution
  - Fees distribution

## Project Structure

```
college-recommendation-system/
├── main.py                 # Main application and recommendation engine
├── data_loader.py         # Data loading and processing module
├── visualization.py       # Visualization module (Matplotlib)
├── colleges_data.csv      # Indian colleges dataset
├── requirements.txt       # Python dependencies
└── README.md             # Project documentation
```

## Prerequisites

- Python 3.6+
- pip (Python package manager)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/alvinthomas398-sys/college-recommendation-system.git
cd college-recommendation-system
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

Run the main application:
```bash
python main.py
```

### Interactive Menu Options

The application provides the following options:

1. **View All Colleges** - Display complete college database
2. **Recommend by Ranking** - Filter colleges by ranking threshold
3. **Recommend by Placement Rate** - Filter by minimum placement percentage
4. **Recommend by State** - Find colleges in a specific state
5. **Recommend by College Type** - Government or Private colleges
6. **Recommend by Budget** - Find affordable colleges within your budget
7. **Multi-Criteria Recommendation** - Combine multiple filters
8. **View Statistics** - See data insights and statistics
9. **View Visualizations** - Generate and view charts
10. **Search College by Name** - Find specific college
11. **Exit** - Close application

## Dataset

The system includes 20 major Indian colleges with the following information:

- **College Name**: Name of the institution
- **Location**: City/Campus location
- **State**: State in India
- **Ranking**: National ranking (1 = top)
- **Average CGPA**: Average GPA of students
- **Placement Rate**: Percentage of students placed
- **Annual Fees**: Annual tuition fee in INR
- **Courses Offered**: Number of courses/programs
- **Type**: Government or Private
- **Entrance Exam**: Required entrance examination

### Sample Colleges Included

- IIT Bombay (Rank #1)
- IIT Delhi (Rank #2)
- IIT Madras (Rank #3)
- BITS Pilani (Rank #7)
- NIT Trichy (Rank #8)
- Delhi University (Rank #10)
- FLAME University (Rank #14)
- CHRIST University (Rank #15)
- And 12 more prestigious institutions

## Modules

### data_loader.py
Handles data loading and processing:
- `CollegeDataLoader`: Main class for data management
- Methods for filtering by ranking, state, type, and more
- Statistical analysis capabilities

### visualization.py
Creates visual representations using Matplotlib:
- `CollegeVisualizer`: Main visualization class
- Multiple chart types: scatter, bar, horizontal bar
- Comparative analysis visualizations

### main.py
Core recommendation engine:
- `CollegeRecommendationSystem`: Main recommendation class
- Interactive user interface
- Multi-criteria filtering logic
- Menu-driven application flow

## Example Usage

### Get Top 5 Colleges
```python
system = CollegeRecommendationSystem()
top_colleges = system.recommend_by_ranking(5)
print(top_colleges)
```

### Find Colleges with 90%+ Placement
```python
system = CollegeRecommendationSystem()
colleges = system.recommend_by_placement(90)
print(colleges)
```

### Multi-Criteria Search
```python
system = CollegeRecommendationSystem()
result = system.multi_criteria_recommendation(
    max_ranking=15,
    min_placement=85,
    college_type='Government',
    max_fees=300000
)
print(result)
```

## Visualizations

The system generates interactive visualizations:

1. **Ranking vs Placement** - Shows correlation between college ranking and placement success
2. **College Type Distribution** - Pie chart of Government vs Private colleges
3. **Top Colleges** - Horizontal bar chart of top-ranked institutions
4. **Placement by Type** - Average placement rates by college type
5. **State Distribution** - Number of colleges per state
6. **Fees Distribution** - Colored scatter plot of college fees vs ranking

## Technical Stack

- **Python 3** - Programming language
- **Pandas** - Data manipulation and analysis
- **Matplotlib** - Data visualization and plotting
- **NumPy** - Numerical computing support

## Key Capabilities

✅ Real-time filtering and recommendations
✅ Multi-criteria search functionality
✅ Comprehensive data analysis
✅ Beautiful visualizations
✅ Budget-friendly recommendations
✅ Geographic filtering
✅ College type selection
✅ Placement rate analysis
✅ Statistical insights

## Future Enhancements

- Add more colleges to the dataset
- Include entrance exam scores data
- Add student reviews and ratings
- Implement machine learning for better recommendations
- Add web interface using Flask/Django
- Include scholarship information
- Add alumni network data
- Integration with official college websites

## Author

Created by: alvinthomas398-sys

## License

This project is open source and available under the MIT License.

## Contributing

Feel free to fork this repository and submit pull requests for improvements!

## Support

For issues or questions, please create an issue in the repository.

---

**Happy College Hunting! 🎓✨**