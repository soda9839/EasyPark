# อ่านก่อนใช้
ไฟล์หลักของ Mobile App อยู่ในโฟลเดอร์ ParkingApp\BookingPark
เมื่อโคลนไปแล้วให้ทำการเข้าไปใน โฟลเดอร์ ParkingApp\BookingPark 
จากนั้นให้ใช้คำสั่ง npm install
จากนั้นให้เข้าไปในโฟลเดอร์ ParkingApp\Setting แล้วทำตาม README ในนั้นเพื่อแก้บัค

********///// ยังไม่ต้องทำ npm i ก็น่าจะมาปกติแล้ว
เอาไฟล์จาก google drive นี้มาใส่ใน part BookingPark\Android
https://drive.google.com/drive/folders/1XWeBbQ0K5iOfuW23p22dcPHV031wAMfd?usp=sharing
********/////
ป.ล. หาก login แล้วเข้าไปสู่หน้า Map แต่กลับขึ้นโหลดแบบไม่มีทีท่าว่าจะหยุดก็ให้ลองเปลี่ยน API ของ Emulator เป็น API 27 หรือต่ำกว่าดู

ป.ล.2 API ต่างๆเก็บไว้ใน  .\ParkingApp\BookingParkApp\.env ก่อนใช้งานให้แก้ API เป็นของที่ใช้ได้ก่อน

ป.ล.3 API ของ Google Maps จะมีอีกจุดหนึ่งเพื่อเปิดใช้งานแผนที่ซึ่งส่วนนี้จะใส่ไว้ใน .\ParkingApp\BookingParkApp\android\app\src\main ไฟล์ AndroidManifest.xml ใน่สวนของ android:value="YOUR_API_KEY"
ที่ YOUR_API_KEY ให้ใช้ API Google ที่เปิดใช้งาน Google map แล้ว
    <!-- Maps -->
    <meta-data
            android:name="com.google.android.geo.API_KEY"
            android:value="YOUR_API_KEY"
            android:usesCleartextTraffic="true"/><!-- end maps -->



*** API GOOGLE MAP  ที่เปิด ***
1. Maps Embed API
2. Maps SDK for Android
3. Places API
4. Maps SDK for iOS
5. Directions API [ถ้าหากต้องการใช้การนำทางใน google map (เสียเงิน)]
6. Distance Matrix API
