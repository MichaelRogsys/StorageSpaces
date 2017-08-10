<h2> DISKSPD.EXE </h2>
<h3> Disk Speed File Used for BenchMarks which can be used on the command line or PowerShell </h3>

 https://gallery.technet.microsoft.com/DiskSpd-a-robust-storage-6cd2f223 
 
 
 <h4> Example Uses </h4>
 <blockquote>
 Command Line:

Diskspd.exe -b8K -d60 -h -L -o2 -t4 -r -w30 -c50M c:\io.dat

PowerShell:

Diskspd.exe -b8K -d60 -h -L -o2 -t4 -r -w30 -c50M c:\io.dat
</blockquote>

Will give a result similar to this:
 <blockquote>
Results for timespan 1:
*******************************************************************************

actual test time:       60.00s
thread count:           4

Total IO
thread |       bytes     |     I/Os     |     MB/s   |  I/O per s |  AvgLat  | LatStdDev |  file
-----------------------------------------------------------------------------------------------------
     0 |        44900352 |         5481 |       0.71 |      91.35 |   21.910 |    27.633 | c:\io.dat (50MB)
     1 |        44720128 |         5459 |       0.71 |      90.98 |   21.987 |    26.877 | c:\io.dat (50MB)
     2 |        44761088 |         5464 |       0.71 |      91.07 |   21.981 |    26.822 | c:\io.dat (50MB)
     3 |        45817856 |         5593 |       0.73 |      93.22 |   21.466 |    26.323 | c:\io.dat (50MB)
-----------------------------------------------------------------------------------------------------
total:         180199424 |        21997 |       2.86 |     366.61 |   21.834 |    26.916

</blockquote>
