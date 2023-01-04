## Data:

Data terdiri dari 5 csv file:
1. megaline_calls.csv
  - `id` — ID sesi web unik
  - `call_date` — tanggal panggilan
  - `duration` — durasi panggilan (dalam menit)
  - `user_id` — ID pengguna yang melakukan panggilan
2. megaline_internet.csv
  - `id` — ID sesi web unik
  - `mb_used` — volume data yang dihabiskan selama sesi (dalam megabita)
  - `session_date` — tanggal sesi web
  - `user_id` — ID pengguna
3. megaline_messages.csv
  - `id` — ID SMS unik
  - `message_date` — tanggal SMS dikirim
  - `user_id` — ID pengguna yang mengirim SMS
4. megaline_plans.csv
  - `plan_name` — nama paket telepon
  - `usd_monthly_fee` — biaya bulanan dalam dolar AS
  - `minutes_included` — alokasi menit panggilan bulanan
  - `messages_included` — alokasi SMS bulanan
  - `mb_per_month_included` — alokasi volume data bulanan (dalam megabita)
  - `usd_per_minute` — harga per menit jika telah melebihi batas alokasi paket (misalnya, jika paket memiliki alokasi 100 menit, maka penggunaan mulai dari menit ke-101 akan dikenakan biaya)
  - `usd_per_message` — harga per SMS jika telah melebihi batas alokasi paket
  - `usd_per_gb` — harga per ekstra gigabita data jika telah melebihi batas alokasi paket (1 GB = 1024 megabita)
5. megaline_users.csv
  - `user_id` — ID pengguna
  - `first_name` — nama depan pengguna
  - `last_name` — nama belakang pengguna
  - `age` — usia pengguna (tahun)
  - `reg_date` — tanggal mulai berlangganan (yyyy-mm-dd)
  - `churn_date` — tanggal pengguna berhenti menggunakan layanan (jika nilainya hilang atau tidak ada, berarti paket layanan sedang digunakan saat data ini dibuat)
  - `city` — kota tempat tinggal pengguna
  - `plan` — nama paket telepon


## Hypothesis:

- Aktivitas pengguna berbeda-beda tergantung pada hari dan kotanya
- Pada Senin pagi penduduk Springfield dan Shelbyville mendengarkan genre yang berbeda
- Pada Jumat malam penduduk Springfield dan Shelbyville mendengarkan genre yang berbeda
- Pendengar di Springfield dan Shelby ville memiliki preferensi musik yang berbeda. Springfield menyukai genre pop sementara Shelbyville menyukai genre rap

## Library:

- pandas
