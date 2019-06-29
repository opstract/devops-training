# Process Priorities Tasks

1. **Create** a new directory under **/tmp** and create **eight** pipes in that directory. 
2. Pick **four** pipes and bounce a character between each pair of these pipes.
3. By using **top** and **ps** display the information **(pid, ppid, priority, nice value, ...)** of these four **cat** processes.
4. **Bounce** another character between the other pairs of pipes, but this time start the commands **nice -5**. **Verify** that all cat processes are battling for the cpu.
5. By using **ps** **verify** that the four new cat processes have a nice value. Use the **-o** and **-C** options of ps for this.
6. **Use** renice to **increase** the nice value from 5 to 10. **Notice** the difference with the usual commands.
