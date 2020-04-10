#!/bin/bash
#SBATCH -N 1
#SBATCH -t 14-00:00:00
#SBATCH -p defq
#SBATCH -o modeltest.out
#SBATCH -e modeltest.err
#SBATCH --mail-type=ALL
#SBATCH --mail-user=your_email_here

module load modeltest-ng

#--- Start the timer
t1=$(date +"%s")

# run this command
modeltest-ng-static -i alignedfile.fasta -h uigf -f ef

#---Complete job
t2=$(date +"%s")
diff=$(($t2-$t1))
echo "[---$SN---] ($(date)) $(($diff / 60)) minutes and $(($diff % 60)) seconds elapsed."
echo "[---$SN---] ($(date)) $SN COMPLETE."
