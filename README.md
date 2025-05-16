# revenue-for-hospitality-domain
# Hotel Booking Analysis

This project aims to analyze hotel booking data to gain insights into customer behavior, room utilization, and revenue generation. The data spans the months of May, June, and July, and includes multiple dimensions and facts related to bookings, hotels, and rooms.

---

## 📂 Dataset Overview

The dataset consists of **five CSV files** and one **metadata file** describing the columns of each CSV.

### 1. `dim_date.csv`
Describes the calendar dimension, helping in time-based analyses.

| Column      | Description                                         |
|-------------|-----------------------------------------------------|
| `date`      | The actual date (spanning May, June, July).         |
| `mmm yy`    | Formatted date as Month Year (e.g., May 25).        |
| `week no`   | Week number of the year.                            |
| `day_type`  | Whether the date falls on a `Weekend` or `Weekday`. |

---

### 2. `dim_hotels.csv`
Provides descriptive details about each hotel.

| Column         | Description                                             |
|----------------|---------------------------------------------------------|
| `property_id`  | Unique ID for each hotel.                               |
| `property_name`| Name of the hotel.                                      |
| `category`     | Hotel class: `Luxury` or `Business`.                    |
| `city`         | City where the hotel is located.                        |

---

### 3. `dim_rooms.csv`
Contains room type and classification data.

| Column       | Description                                                    |
|--------------|----------------------------------------------------------------|
| `room_id`    | Room type (`RT1`, `RT2`, `RT3`, `RT4`).                         |
| `room_class` | Class of room: `Standard`, `Elite`, `Premium`, `Presidential`. |

---

### 4. `fact_aggregated_bookings.csv`
Aggregated data for bookings on a per-day, per-hotel, per-room basis.

| Column              | Description                                                       |
|---------------------|-------------------------------------------------------------------|
| `property_id`       | Hotel ID.                                                         |
| `check_in_date`     | Date when guests checked in.                                      |
| `room_category`     | Type of room booked (`RT1`, `RT2`, etc.).                         |
| `successful_bookings`| Number of successful bookings for that room on that date.        |
| `capacity`          | Maximum number of rooms available for that category on that date. |

---

### 5. `fact_bookings.csv`
Detailed booking transactions.

| Column            | Description                                                                                      |
|-------------------|--------------------------------------------------------------------------------------------------|
| `booking_id`      | Unique ID for each booking.                                                                      |
| `property_id`     | Hotel ID.                                                                                        |
| `booking_date`    | Date when the booking was made.                                                                  |
| `check_in_date`   | Guest check-in date.                                                                             |
| `check_out_date`  | Guest check-out date.                                                                            |
| `no_guests`       | Number of guests staying in the room.                                                            |
| `room_category`   | Type of room booked (`RT1`, `RT2`, etc.).                                                        |
| `booking_platform`| Platform used to make the booking.                                                               |
| `ratings_given`   | Rating provided by the guest.                                                                    |
| `booking_status`  | Status of the booking: `Cancelled`, `Checked Out`, or `No Show`.                                 |
| `revenue_generated`| Revenue earned from the booking.                                                                |
| `revenue_realized`| Final revenue after deductions (e.g., cancellations result in 40% refund).                       |

---

## 📸 Screenshot

![Project Screenshot](path/to/your/screenshot.png)

> Replace the above path with your actual screenshot file path or image URL.

---

## 🧠 Objective

This project is designed to:
- Understand booking patterns across different room types and hotel categories.
- Analyze customer behavior including booking platforms, ratings, and cancellation patterns.
- Evaluate hotel performance in terms of capacity utilization and revenue realization.

---

## 🛠️ Tech Stack

- Python (Pandas, NumPy, Matplotlib/Seaborn)
- Jupyter Notebook
- Git & GitHub

---

## 📈 Future Work

- Integrate machine learning for demand forecasting.
- Build dashboards using Tableau or Power BI.
- Optimize pricing strategy based on customer and seasonal trends.

---

## 🤝 Contributing

Feel free to fork this repository and contribute via pull requests!

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

