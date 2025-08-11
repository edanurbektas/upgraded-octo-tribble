-- 1. Sahte müşteri tablosu oluşturma CREATE TABLE Customers ( CustomerID INT PRIMARY KEY, FirstName VARCHAR(50), LastName VARCHAR(50), Email VARCHAR(100), City VARCHAR(50), Country VARCHAR(50) );

-- 2. Sahte veriler ekleme INSERT INTO Customers (CustomerID, FirstName, LastName, Email, City, Country) VALUES (1, 'Ali', 'Yılmaz', 'ali.yilmaz@example.com', 'İstanbul', 'Türkiye'), (2, 'Ayşe', 'Kara', 'ayse.kara@example.com', 'Ankara', 'Türkiye'), (3, 'Mehmet', 'Demir', 'mehmet.demir@example.com', 'İzmir', 'Türkiye'), (4, 'Elif', 'Şahin', 'elif.sahin@example.com', 'Bursa', 'Türkiye'), (5, 'Ahmet', 'Çelik', 'ahmet.celik@example.com', 'Antalya', 'Türkiye');

-- 3. Basit SQL sorguları örnekleri -- Tüm müşteri kayıtlarını listeleme SELECT * FROM Customers;

-- Sadece İstanbul'daki müşterileri getirme SELECT * FROM Customers WHERE City = 'İstanbul';

-- E-posta adresinde "example" geçen müşterileri getirme SELECT * FROM Customers WHERE Email LIKE '%example%';

-- Şehre göre müşteri sayısını gruplama SELECT City, COUNT(*) AS CustomerCount FROM Customers GROUP BY City;

-- Belirli bir müşteriyi ID ile arama SELECT * FROM Customers WHERE CustomerID = 3;

