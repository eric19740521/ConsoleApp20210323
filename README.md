VS2017 C# MYSQL��Ʈw�}�o(�D���x���ε{��)

�ѦҸ��:
https://docs.microsoft.com/zh-tw/azure/mysql/connect-csharp
http://yhhuang1966.blogspot.com/2017/11/xampp-php.html
http://www.coolsun.idv.tw/modules/xhnewbb/viewtopic.php?topic_id=1510
https://anglerdiy.com/?p=2563
https://ithelp.ithome.com.tw/articles/10218214


1.xampp,mysql�w��
http://yhhuang1966.blogspot.com/2017/11/xampp-php.html


2.mySQL�޲z�u��(Navicat_Portable_v12.0.17/phpMyAdmin)
https://softblog.tw/navica.html



3.vs2017 �w��
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



ExecuteScalar�]�^�Ȫ�^�d�߲Ĥ@��Ĥ@�C���ȡC
ExecuteReader�]�^��^�@�ӹ�H�A�ӹ�H�i�H���N��ӵ��G���A�P�ɥu�b���s���O�d�@���O���C
ExecuteNonQuery�]�^�ڥ�����^�ƾڡG�u�������J�A��s�ΧR���v�T����ơC

ExecuteScalar��z�եΤ@��SQL�жq��ƮɡA���u��^�@�ӼƦr�C
ExecuteReader��z���b�i��SQL�եήɡA�N�q����^�@�ӰO�����A�o�N?�z���Ѥ@��SqlDataReader��H���˯�C�������ƾڡC
ExecuteNonQuery�Ω�S������������SQL�A�Ⱦ���^�ȮɡA�Ҧp�@��²�檺UPDATE�y�y�C

