## Data:

Data terdiri dari 5 csv file:
- megaline_calls.csv
  - `id` — ID sesi web unik
  - `call_date` — tanggal panggilan
  - `duration` — durasi panggilan (dalam menit)
  - `user_id` — ID pengguna yang melakukan panggilan
- megaline_internet.csv
  - `id` — ID sesi web unik
  - `mb_used` — volume data yang dihabiskan selama sesi (dalam megabita)
  - `session_date` — tanggal sesi web
  - `user_id` — ID pengguna
- megaline_messages.csv
  - `id` — ID SMS unik
  - `message_date` — tanggal SMS dikirim
  - `user_id` — ID pengguna yang mengirim SMS
- megaline_plans.csv
  - `plan_name` — nama paket telepon
  - `usd_monthly_fee` — biaya bulanan dalam dolar AS
  - `minutes_included` — alokasi menit panggilan bulanan
  - `messages_included` — alokasi SMS bulanan
  - `mb_per_month_included` — alokasi volume data bulanan (dalam megabita)
  - `usd_per_minute` — harga per menit jika telah melebihi batas alokasi paket (misalnya, jika paket memiliki alokasi 100 menit, maka penggunaan mulai dari menit ke-101 akan dikenakan biaya)
  - `usd_per_message` — harga per SMS jika telah melebihi batas alokasi paket
  - `usd_per_gb` — harga per ekstra gigabita data jika telah melebihi batas alokasi paket (1 GB = 1024 megabita)
- megaline_users.csv
  - `user_id` — ID pengguna
  - `first_name` — nama depan pengguna
  - `last_name` — nama belakang pengguna
  - `age` — usia pengguna (tahun)
  - `reg_date` — tanggal mulai berlangganan (yyyy-mm-dd)
  - `churn_date` — tanggal pengguna berhenti menggunakan layanan (jika nilainya hilang atau tidak ada, berarti paket layanan sedang digunakan saat data ini dibuat)
  - `city` — kota tempat tinggal pengguna
  - `plan` — nama paket telepon


## Goals:
- Menganalisis perilaku klien dan menentukan paket prabayar mana yang mendatangkan lebih banyak pendapatan

## Step:
- Pengecekan Kualitas Data
- Modifikasi Data
- Analisis Data; Mendeskripsikan perilaku konsumen
- Uji Hipotesis
  - Rata-rata pendapatan dari pengguna paket telepon Ultimate dan Surf berbeda
  - Rata-rata pendapatan dari pengguna di wilayah NY-NJ berbeda dengan pendapatan pengguna dari wilayah lain


## Library:

- pandas
- matplotlib.pyplot
- seaborn
- numpy
- scipy.stats
