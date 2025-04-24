# Proyek Akhir: Menyelesaikan Permasalahan Perusahaan Edutech

## Business Understanding

PT.Jaya Jaya Maju menggalami peningkatan karyawan yang berhenti(_Attrition_) sebesar **12%** dari total karyawan yang ada. Untuk mengetahui apa penyebab tingginya _attrition_, maka diperlukan analisis menyelasaikan masalah yang sedang dialami oleh perusahaan.

### Permasalahan Bisnis

Faktor apa saja yang menjadi kendala utama tingginya _attrition rate_ yang dialami oleh PT. Jaya Jaya Maju?

### Cakupan Proyek

Untuk mencari faktor-faktor penyebab tingginya _attrition rate_, diperlukan analisis dengan menggunakan visualisasi data. Kemudian membuat dashboard berdasarkan temuan yang didapatkan melalui analisis yang sudah dilakukan.

### Persiapan

**Sumber data**: [Employee data](https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee)  
Daftar kolom yang terdapat pada dataset:
* EmployeeId - Employee Identifier
* Attrition - Did the employee attrition? (0=no, 1=yes)
* Age - Age of the employee
* BusinessTravel - Travel commitments for the job
* DailyRate - Daily salary
* Department - Employee Department
* DistanceFromHome - Distance from work to home (in km)
* Education - 1-Below College, 2-College, 3-Bachelor, 4-Master,5-Doctor
* EducationField - Field of Education
* EnvironmentSatisfaction - 1-Low, 2-Medium, 3-High, 4-Very High
* Gender - Employee's gender
* HourlyRate - Hourly salary
* JobInvolvement - 1-Low, 2-Medium, 3-High, 4-Very High
* JobLevel - Level of job (1 to 5)
* JobRole - Job Roles
* JobSatisfaction - 1-Low, 2-Medium, 3-High, 4-Very High
* MaritalStatus - Marital Status
* MonthlyIncome - Monthly salary
* MonthlyRate - Mounthly rate
* NumCompaniesWorked - Number of companies worked at
* Over18 - Over 18 years of age?
* OverTime - Overtime?
* PercentSalaryHike - The percentage increase in salary last year
* PerformanceRating - 1-Low, 2-Good, 3-Excellent, 4-Outstanding
* RelationshipSatisfaction - 1-Low, 2-Medium, 3-High, 4-Very High
* StandardHours - Standard Hours
* StockOptionLevel - Stock Option Level
* TotalWorkingYears - Total years worked
* TrainingTimesLastYear - Number of training attended last year
* WorkLifeBalance - 1-Low, 2-Good, 3-Excellent, 4-Outstanding
* YearsAtCompany - Years at Company
* YearsInCurrentRole - Years in the current role
* YearsSinceLastPromotion - Years since the last promotion
* YearsWithCurrManager - Years with the current manager


**Setup environment**:  
library yang digunakan untuk analisis data:
```
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

## Business Dashboard

**Link Dashboard** : [LookerStudio-Dashboard](https://lookerstudio.google.com/u/0/reporting/ef868bae-f17f-471e-b8d2-5fd997eb6f12/page/B81aE)  
![Local Image](ichsanelf-dashboard.JPG)    

Dashboard ini dibuat dengan menggunakan **Looker Studio**. Grafik-grafik yang terdapat pada dashboard memiliki informasi seperti:
1. Jumlah karyawan. 
2. Sebuah _filter Attrition_(Yes/No), untuk mengatur visualisasi dari _chart_ yang tersedia.
3. Jumlah departemen yang dimiliki perusahaan beserta jumlah karyawan yang terdapat pada masing-masing departemen.
4. Posisi karyawan disetiap departemen yang ada.
5. Jenis kelamin, status nikah, dan umur karyawan. Grafik ini bisa diubah-ubah dengan menggunakan tanda panah yang ada dipojok kanan atas. Untuk melihat status nikah dan umur karyawan berdasarkan kelompok umur.
6. Grafik untuk faktor-faktor _Attrition_. Sama seperti grafik jenis kelamin/status nikah/umur, grafik ini bisa diubah-ubah. Pada grafik ini memiliki informasi, yaitu:
    * Years With Current manager
    * Number of Training Since Last Year 
	* Promotion Since Last year
	* Salary Hike
	* Overtime
	* Enviroment Satisfaction
	* Job Satisfaction
	* Job Involvement
	* Work Life Balance
## Conclusion

Hasil analisis menunjukkan faktor-faktor yang menunjukkan tingginya _Attrition rate_, adalah sebagai berikut:
1. Terdapat **137** karyawan yang bekerja kurang dari lima tahun dibawah managernya saat yang keluar dari perusahaan.
2. Sebanyak **98** karyawan yang memiliki _overtime_ keluar dari perusahaan.
3. **78** karyawan yang tidak memiliki kenaikan gaji secara signifikan sejak tahun lalu keluar dari perusahaan.
4. **141** karyawan yang hanya menerima pelatihan kurang dari tiga kali selama setahun keluar dari perusahaan.
5. Karyawan yang keluar dari perusahaan sebanyak **153** tidak menerima promosi semenjak setahun terakhir.

Dengan _Attrition rate_ sebesar **12%** atau **179** orang yang keluar dari perusahaan, tentunya ini menjadi hal menghawatirkan. Terutama dari jumlah tersebut, banyak karyawan yang memiliki performa yang tinggi, yaitu **151** orang memiliki _excellent_ dan **28** _outstanding performance_. Lalu, sebanyak **92** orang memiliki peran aktif dalam pekerjaan mereka. 


### Rekomendasi Action Items (Optional)

Yang perlu dilakukan oleh perusahaan untuk menyelesaikan masalah ini, perusahaan perlu memfokuskan pada faktor-faktor seperti:
* **Hubungan kerja antara karyawan dengan manager.**  
Dengan angka sebesar **137** orang, perusahaan perlu memperhatikan hubungan kerja antara manager dan karyawan yang bekerja dibawah mereka. Karena sudah tentunya komunikasi yang baik antara atasan dan bawahan menjadi modal penting untuk berjalannya sebuah perusahaan

* **Pelatihan kerja untuk karyawan.**
Karyawan juga memerlukan motivasi dengan memberikan pelatihan untuk meningkatkan performa mereka. Pelatihan menurut saya tidak hanya untuk karyawan yang memiliki performa rendah, tapi juga yang memiliki performa tinggi atau menenggah. Karena dengan memberikan pelatihan, dapat memberikan motivasi untuk menjadi lebih baik dan juga merasa bahwa mereka dipercaya dan dibutuhkan oleh perusahaan. Dan tentunya juga bisa meningkatkan relasi antara karyawan dengan perusahaan menjadi lebih baik.  

* **Promosi atau kenaikkan posisi karyawan dalam perusahaan.**  
Dan untuk poin terakhir, walau promosi menurut saya sebenarnya mungkin tidak bisa dieksekusi dengan mudah. Namun, perlu dipertimbangkan dengan melihat bahwa dari total **12%** atau **179** karyawan yang berhenti. Mereka memiliki performa pekerjaan yang tinggi, yang tentunya mereka adalah aset terbesar dari perusahaan jika mereka tetap bertahan di perusahaan. Dengan melihat sebanyak **153** dalam setahun terakhir ini mereka tidak mendapatkan sebuah promosi. Sudah tentunya perusahaan perlu mempertimbangkan posisi mereka dalam perusahaan. Apakah mereka pantas atau tidak mendapatkan sebuah promosi atau juga kenaikkan gaji.

* **Overtime atau jam lembur**  
Walau angka karyawan yang keluar karena faktor ini cukup rendah. Namun hal ini tidak dapat diabaikan, karena kenapa karyawan memilih keluar. Apakah mereka tidak dapat gaji yang sesuai? Atau kondisi jam lembur yang terlalu berat?. Maka perusahaan perlu melihat apa yang menjadi masalah pada jam lembur. Solusi seperti mengurangi jam lembur dapat dilakukan jika memang memungkinkan. Jika masalah tersebut tidak dapat diatasi, tentunya bisa meningkatkan _attrition_ dimasa depan.
