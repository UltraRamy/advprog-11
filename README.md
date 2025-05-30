# Refleksi 1

1. Sebelum diekspos sebagai Service, log hanya mencatat akses lokal. Setelah jadi Service, log mencatat akses dari IP cluster. Setiap kali aplikasi dibuka lewat proxy, log bertambah. Ini menandakan akses berhasil diteruskan oleh Service. Jumlah log naik tiap kali app diakses. Service bekerja sesuai fungsinya.

2. Opsi -n digunakan untuk menentukan namespace. Tanpa -n, kubectl get hanya menampilkan resource di namespace default. Namespace memisahkan resource agar tidak tercampur. Bagian kube-system berisi komponen internal Kubernetes. Resource yang kamu buat ada di namespace lain, misalnya default. Itulah sebabnya tidak muncul saat pakai -n kube-system.
