# Currency Apps
Aplikasi mencakup fungsi perhitungan nilai tukar mata uang dari dollar ke rupiah. satu dollar dianggap senilai Rp.15.000

## Scope & Functionalities
-  user dapat memasukkan angka
-  user dapat menyentuh tombol hitung
-  user mendapat info "INVALID" yang dimasukkan berupa text

## How Does it works?
diawali dengan method "MainWindow"
``` csharp
    public MainWindow()
        {
            InitializeComponent();
            currencyController = new CurrencyController();

        }
```

logika perhitungan terdapat pada class `CurrencyController.cs` sebagai berikut
``` csharp
 public string usdToIdr(string nominal)
        {
            var nominalDouble = Convert.ToDouble(nominal);
            var result = nominalDouble * 15000;
            return Convert.ToString(result);
        }
```
