trigger-code-..
===============


import sys
import shutil
import time

def main():
    sys.path.append("/home/desktop/anit/zivame")
    directory = "/home/desktop/anit/zivame/zivame_dir"


    directory2 = "%s%s" %(directory, time.strftime("%d%m%y"))
    
    import code1_first_zivame
    code1_first_zivame.main(directory)
    code1_first_zivame.main2(directory)

    import csv_store
    csv_store.main(directory)

    import insert_update
    insert_update.supermain()

    import mysql_con_python_junglee2
    mysql_con_python_junglee2.supermain()


    import mysql_con_python_junglee4
    mysql_con_python_junglee4.supermain()

    #import to_my_sql_junglee
    #to_my_sql_junglee.supermain(directory)


    #########import mysql_con_python_junglee3
    #########mysql_con_python_junglee3.supermain()

    #########import to_my_sql_junglee3
    ########to_my_sql_junglee3.supermain(directory)

    import upload_to_cdn
    upload_to_cdn.supermain(directory)

    import code6_first_to_cmmn_myntra
    code6_first_to_cmmn_myntra.supermain()
    
    shutil.move(directory, directory2)




if __name__=="__main__":
    main()
