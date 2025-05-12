# 📈 Student Grade Improvement Recommendation System

This project provides personalized, AI-driven suggestions to help students improve their academic performance based on their current habits and lifestyle factors.

## 🔍 Project Objective

By analyzing a student's current grade, target score, and personal behavioral data, this system:

- Identifies the **most impactful features** affecting performance,
- Recommends **actionable changes** to reach the target grade more effectively.

Ideal for educational consultants, academic coaches, or self-driven learners.

## 🧠 Model and Features

The system uses a trained machine learning model to analyze features such as:

- `study_hours_per_day`: Daily study time
- `social_media_hours`: Daily time spent on social media
- `netflix_hours`: Daily Netflix watch time
- `sleep_hours`: Average hours of sleep per day
- `exercise_frequency`: Weekly exercise sessions

The model evaluates each feature's importance and generates recommendations based on the top 5 most influential variables.

## 🚀 Usage

```python
get_improvement_recommendations(current_score=65, target_score=80, student_features={
    "study_hours_per_day": 2,
    "social_media_hours": 3,
    "netflix_hours": 2,
    "sleep_hours": 6,
    "exercise_frequency": 1
})
[
  "By increasing your study time by 1 hour per day, you could potentially improve your grade by approximately 12.5%.",
  "Reducing social media usage by 1 hour daily may boost your grade by around 9.8%.",
  "Increasing your sleep duration by 1 hour daily might lead to a 7.4% improvement in performance."
]
