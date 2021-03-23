VS2017 C# MYSQL資料庫開發(主控台應用程式)

參考資料:
https://docs.microsoft.com/zh-tw/azure/mysql/connect-csharp
http://yhhuang1966.blogspot.com/2017/11/xampp-php.html
http://www.coolsun.idv.tw/modules/xhnewbb/viewtopic.php?topic_id=1510
https://anglerdiy.com/?p=2563
https://ithelp.ithome.com.tw/articles/10218214


1.xampp,mysql安裝
http://yhhuang1966.blogspot.com/2017/11/xampp-php.html


2.mySQL管理工具(Navicat_Portable_v12.0.17/phpMyAdmin)
https://softblog.tw/navica.html



3.vs2017 安裝
https://my.visualstudio.com/Downloads?q=visual%20studio%202017&wt.mc_id=o~msft~vscom~older-downloads


3.
DROP PROCEDURE IF EXISTS 'sp01';
DELIMITER //
CREATE PROCEDURE 'sp01'(IN mem_name varchar(20))
main:BEGIN
    SELECT *
    FROM 'member' 
    WHERE 'mem_name' like mem_name;
END
//
DELIMITER ;



ExecuteScalar（）僅返回查詢第一行第一列的值。
ExecuteReader（）返回一個對象，該對象可以迭代整個結果集，同時只在內存中保留一條記錄。
ExecuteNonQuery（）根本不返回數據：只有受插入，更新或刪除影響的行數。

ExecuteScalar當您調用一個SQL標量函數時，它只返回一個數字。
ExecuteReader當您正在進行SQL調用時，將從表中返回一個記錄集，這將?您提供一個SqlDataReader對象來檢索C＃中的數據。
ExecuteNonQuery用於沒有任何類型的SQL服務器返回值時，例如一個簡單的UPDATE語句。

