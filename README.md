# Simple-FileSystem
This is an implementation of simple file system which supports following commands:
   1.  $myfs /* execute the program */
   2.  myfs> /* prompt given by this program */
   3.  myfs>mkfs osfile1 512 10 /* creates the filesystem on file osfile1, blocksize is taken to be 512B */
   4.  myfs>mkfs osfile2 1024 20 /* creates the filesystem on file osfile2, blocksize is taken to be 1024B */
   5.  myfs>use osfile1 as C: /* the filesystem on osfile1 will henceforth be accessed as C: */
   6.  myfs>use osfile2 as D: /* the filesystem on osfile2 will henceforth be accessed as D: */
   7.  myfs>cp osfile3 C:tesfile1 /* copy the file osfile3 from os to the filesystem C: as testfile1 */
   8.  myfs>ls C: /* see the contents of the filesystem C: */
    		testfile1 ... size
   9.  myfs>cp C:tesfile1 C:testfile1a /* copy the file testfile1 from C: to the filesystem C: as testfile1a */
   10. myfs>ls C: /* see the contents of the filesystem C: */
     		testfile1 ... size
    		testfile1a ... size
   11.  myfs>cp C:tesfile1 D:testfile2 /* copy the file testfile1 from C: to the filesystem D: as testfile2 */
   12.  myfs>cp D:testfile2 osfile4 /* copy the file testfile2 from C: to the to the OS as osfile4 */
   13.  myfs>rm C:testfile1 /* Delete the testfile1 from C: */
   14.  myfs>ls C: /* see the contents of the filesystem C: */ 
   		  testfile1a ... size
   15.  myfs>mv D:testfile2 D:testfile2a  /* Rename  testfile2 of D: to testfile2a in D: */ 
   16.  myfs>info /*This will show all information about existing file-systems that we have created so far*/
   17.  myfs>clear /*Clear the terminal*/
   18.  myfs>exit /* terminate the process */

#NOTE:
	After modifying the file system do not terminate the process using [ctrl+c]. Always use "exit" to close the programme.
