<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Input Absensi Siswa</title>
    <!-- Memuat Tailwind CSS untuk styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Menggunakan font Inter sebagai default */
        body {
            font-family: 'Inter', sans-serif;
        }
        /* Style untuk dropdown autocomplete */
        .autocomplete-items {
            position: absolute;
            border: 1px solid #d4d4d4;
            border-bottom: none;
            border-top: none;
            /* Menaikkan z-index untuk memastikan tampil di atas elemen lain di mobile */
            z-index: 999;
            top: 100%;
            left: 0;
            right: 0;
            max-height: 150px;
            overflow-y: auto;
        }
        .autocomplete-items div {
            padding: 10px;
            cursor: pointer;
            background-color: #fff;
            border-bottom: 1px solid #d4d4d4;
        }
        .autocomplete-items div:hover {
            background-color: #e9e9e9;
        }
        .autocomplete-active {
            background-color: DodgerBlue !important;
            color: #ffffff;
        }
    </style>
</head>
<body class="bg-gray-100 flex items-center justify-center min-h-screen">

    <!-- Menambahkan padding bawah (pb-8) untuk memberi ruang di mobile -->
    <div class="w-full max-w-lg bg-white rounded-xl shadow-lg p-8 m-4 pb-8">
        <div id="message-container" class="hidden mb-4 p-4 text-sm rounded-lg"></div>
        <h1 class="text-2xl font-bold text-center text-gray-800 mb-2">Formulir Absensi Siswa</h1>
        <p class="text-center text-gray-500 mb-6">Silakan pilih kelas, lalu ketik nama siswa.</p>

        <form id="absensiForm" class="space-y-6">

            <!-- Pilihan Kelas dengan Dropdown Manual -->
            <div>
                <label for="kelas" class="block text-sm font-medium text-gray-700 mb-1">Pilih Kelas</label>
                <select id="kelas" name="kelas" required class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 transition duration-150 bg-white">
                    <option value="" disabled selected>-- Pilih Kelas --</option>
                    <optgroup label="Kelas 7">
                        <option value="7.1">7.1</option>
                        <option value="7.2">7.2</option>
                        <option value="7.3">7.3</option>
                        <option value="7.4">7.4</option>
                        <option value="7.5">7.5</option>
                        <option value="7.6">7.6</option>
                    </optgroup>
                    <optgroup label="Kelas 8">
                        <option value="8.1">8.1</option>
                        <option value="8.2">8.2</option>
                        <option value="8.3">8.3</option>
                        <option value="8.4">8.4</option>
                        <option value="8.5">8.5</option>
                        <option value="8.6">8.6</option>
                    </optgroup>
                    <optgroup label="Kelas 9">
                        <option value="9.1">9.1</option>
                        <option value="9.2">9.2</option>
                        <option value="9.3">9.3</option>
                        <option value="9.4">9.4</option>
                        <option value="9.5">9.5</option>
                    </optgroup>
                </select>
            </div>

            <!-- Input Nama dengan Autocomplete -->
            <div class="relative">
                <label for="nama" class="block text-sm font-medium text-gray-700 mb-1">Nama Lengkap</label>
                <input type="text" id="nama" name="nama" placeholder="Pilih kelas terlebih dahulu" required class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 transition duration-150" autocomplete="off" disabled>
                <div id="autocomplete-list" class="autocomplete-items"></div>
            </div>

            <!-- Input NISN (otomatis terisi) -->
            <div>
                <label for="nisn" class="block text-sm font-medium text-gray-700 mb-1">NISN</label>
                <input type="number" id="nisn" name="nisn" placeholder="NISN akan terisi otomatis" required readonly class="w-full px-4 py-2 border border-gray-300 rounded-lg bg-gray-100 cursor-not-allowed">
            </div>

            <!-- Input Tanggal (otomatis terisi) -->
            <div>
                <label for="tanggal" class="block text-sm font-medium text-gray-700 mb-1">Tanggal Absensi</label>
                <input type="date" id="tanggal" name="tanggal" required readonly class="w-full px-4 py-2 border border-gray-300 rounded-lg bg-gray-100 cursor-not-allowed">
            </div>

            <!-- Pilihan Keterangan -->
            <div>
                <label for="keterangan" class="block text-sm font-medium text-gray-700 mb-1">Keterangan</label>
                <select id="keterangan" name="keterangan" required class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500 transition duration-150 bg-white">
                    <option value="" disabled selected>Pilih Keterangan</option>
                    <option value="sakit">Sakit</option>
                    <option value="izin">Izin</option>
                    <option value="alfa">Alfa</option>
                </select>
            </div>

            <!-- Tombol Aksi -->
            <div class="flex items-center justify-end space-x-4 pt-2">
                <button type="reset" id="resetBtn" class="px-6 py-2 border border-gray-300 rounded-lg text-sm font-medium text-gray-700 hover:bg-gray-50 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-400 transition duration-150">
                    Reset
                </button>
                <button type="submit" id="submitBtn" class="px-6 py-2 border border-transparent rounded-lg shadow-sm text-sm font-medium text-white bg-blue-600 hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500 transition duration-150 flex items-center justify-center">
                    Kirim
                </button>
            </div>
        </form>
    </div>

    <script>
        // --- KONFIGURASI ---
        // URL Web App dari Google Apps Script Anda sudah dimasukkan di sini.
        const SCRIPT_URL = "https://script.google.com/macros/s/AKfycbzYaxtCxvQ5PY0rioL523e-ZQaPEYpQ5BMfVMpmgnlUvtFBVJAmarfg-KJuiRHJZ5tI/exec";

        // --- Elemen DOM ---
        const kelasSelect = document.getElementById('kelas');
        const namaInput = document.getElementById('nama');
        const nisnInput = document.getElementById('nisn');
        const tanggalInput = document.getElementById('tanggal');
        const autocompleteList = document.getElementById('autocomplete-list');
        const form = document.getElementById('absensiForm');
        const resetBtn = document.getElementById('resetBtn');
        const submitBtn = document.getElementById('submitBtn');
        const messageContainer = document.getElementById('message-container');

        let studentData = {};
        let currentStudents = [];
        let selectedClass = null;
        
        // --- Fungsi Utama ---
        document.addEventListener('DOMContentLoaded', () => {
            setCurrentDate();
            fetchStudentData();
        });

        async function fetchStudentData() {
            try {
                const response = await fetch(SCRIPT_URL);
                const result = await response.json();
                
                if (result.success) {
                    processStudentData(result.data);
                } else {
                    showMessage('Gagal memuat data siswa: ' + result.message, 'error');
                }
            } catch (error) {
                showMessage('Terjadi kesalahan jaringan saat memuat data. Pastikan URL Web App benar dan sudah di-deploy.', 'error');
            }
        }

        function processStudentData(data) {
            // Mengelompokkan siswa berdasarkan kelas untuk autocomplete
            studentData = data.reduce((acc, student) => {
                const key = student.class;
                if (!acc[key]) {
                    acc[key] = [];
                }
                acc[key].push({ name: student.name, nisn: student.nisn });
                return acc;
            }, {});
        }
        
        function setCurrentDate() {
            const today = new Date();
            const year = today.getFullYear();
            const month = String(today.getMonth() + 1).padStart(2, '0');
            const day = String(today.getDate()).padStart(2, '0');
            tanggalInput.value = `${year}-${month}-${day}`;
        }
        
        function showMessage(message, type = 'success') {
            messageContainer.textContent = message;
            messageContainer.className = `mb-4 p-4 text-sm rounded-lg ${type === 'success' ? 'bg-green-100 text-green-800' : 'bg-red-100 text-red-800'}`;
            messageContainer.classList.remove('hidden');
            setTimeout(() => {
                 messageContainer.classList.add('hidden');
                 messageContainer.textContent = '';
            }, 5000);
        }

        // --- Event Listeners ---
        kelasSelect.addEventListener('change', (e) => {
            selectedClass = e.target.value;
            currentStudents = studentData[selectedClass] || [];
            namaInput.disabled = false;
            namaInput.value = '';
            nisnInput.value = '';
            namaInput.placeholder = `Ketik nama siswa kelas ${selectedClass}...`;
            namaInput.focus();
        });

        namaInput.addEventListener('input', function() {
            const value = this.value;
            closeAllLists();
            if (!value || !selectedClass) return;
            
            autocompleteList.innerHTML = '';
            
            currentStudents
                .filter(student => student.name.toLowerCase().includes(value.toLowerCase()))
                .forEach(student => {
                    const item = document.createElement('div');
                    item.innerHTML = `<strong>${student.name.substr(0, value.length)}</strong>${student.name.substr(value.length)}`;
                    item.dataset.name = student.name;
                    item.dataset.nisn = student.nisn;
                    
                    // FUNGSI UNTUK MEMILIH ITEM
                    const selectItemAction = function(e) {
                        e.preventDefault(); // Mencegah perilaku default (seperti kehilangan fokus input)
                        namaInput.value = item.dataset.name;
                        nisnInput.value = item.dataset.nisn;
                        closeAllLists();
                    };

                    // MENAMBAHKAN EVENT LISTENER UNTUK MOUSE DAN SENTUHAN (MOBILE)
                    item.addEventListener('mousedown', selectItemAction);
                    item.addEventListener('touchstart', selectItemAction);
                    
                    autocompleteList.appendChild(item);
                });
        });
        
        form.addEventListener('submit', async (e) => {
            e.preventDefault();
            submitBtn.disabled = true;
            submitBtn.textContent = 'Mengirim...';

            const formData = {
                kelas: form.elements.kelas.value,
                nama: form.elements.nama.value,
                nisn: form.elements.nisn.value,
                tanggal: form.elements.tanggal.value,
                keterangan: form.elements.keterangan.value,
            };

            // Validasi sederhana
            if(!formData.kelas || !formData.nama || !formData.nisn || !formData.keterangan){
                showMessage('Harap lengkapi semua data sebelum mengirim.', 'error');
                submitBtn.disabled = false;
                submitBtn.textContent = 'Kirim';
                return;
            }

            try {
                 const response = await fetch(SCRIPT_URL, {
                    method: 'POST',
                    mode: 'no-cors', 
                    cache: 'no-cache',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(formData),
                    redirect: 'follow'
                });

                showMessage('Absensi berhasil disimpan!', 'success');
                form.reset();
                resetFormState();
                
            } catch (error) {
                 showMessage('Terjadi kesalahan saat mengirim data.', 'error');
            } finally {
                submitBtn.disabled = false;
                submitBtn.textContent = 'Kirim';
            }
        });

        resetBtn.addEventListener('click', () => {
             form.reset();
             resetFormState();
        });

        function resetFormState() {
            closeAllLists();
            namaInput.disabled = true;
            namaInput.placeholder = 'Pilih kelas terlebih dahulu';
            nisnInput.value = '';
            kelasSelect.selectedIndex = 0;
            setTimeout(setCurrentDate, 0); 
            form.elements.keterangan.selectedIndex = 0;
        }

        function closeAllLists() {
            autocompleteList.innerHTML = '';
        }

        document.addEventListener("click", (e) => {
            if (e.target !== namaInput) closeAllLists();
        });

    </script>
</body>
</html>

