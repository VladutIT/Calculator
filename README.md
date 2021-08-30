using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Calculator
{
    public partial class Form1 : Form
    {
        double rezultat = 0, copie = 0;
        char a='#';
        double nr = 0;
        int ok = 0;
        int cnt = 0;////// valorile cnt 1 2 3 si 4
        
        public Form1()
        {
            InitializeComponent();
            ecran.Text = "";
        }

        private void Form1_Load(object sender, EventArgs e)
        {
            
        }

        private void inmultire_Click(object sender, EventArgs e)
        {
            a = '*';
            ok = 1;
            if(cnt!=0)
            {
                if(cnt==1)
                {
                    rezultat = rezultat * nr;
                }
                if(cnt==2)
                {
                    rezultat = rezultat + nr;
                }
                if(cnt==3)
                {
                    rezultat = rezultat / nr;
                }
                if(cnt==4)
                {
                    rezultat = rezultat - nr;
                }
                ecran.Text = "" + rezultat;
                cnt = 0;
                nr = 0;
            }
            cnt=1;
            ecran.Text = ecran.Text + " *";
        }

        private void unu_Click(object sender, EventArgs e)
        {
           
           if(rezultat!=0 && ok==1)
            {
                nr = nr * 10 + 1;
                copie = nr;
            }
           else
            {
                rezultat = rezultat * 10 + 1;
                copie = rezultat;
            }
            ecran.Text = "" + copie;
        }

        private void doi_Click(object sender, EventArgs e)
        {

            if (rezultat != 0 && ok == 1)
            {
                nr = nr * 10 + 2;
                copie = nr;
            }
            else
            {
                rezultat = rezultat * 10 + 2;
                copie = rezultat;
            }
            ecran.Text = "" + copie;
        }

        private void trei_Click(object sender, EventArgs e)
        {

            if (rezultat != 0 && ok == 1)
            {
                nr = nr * 10 + 3;
                copie = nr;
            }
            else
            {
                rezultat = rezultat * 10 + 3;
                copie = rezultat;
            }
            ecran.Text = "" + copie;
        }

        private void patru_Click(object sender, EventArgs e)
        {

            if (rezultat != 0 && ok == 1)
            {
                nr = nr * 10 + 4;
                copie = nr;
            }
            else
            {
                rezultat = rezultat * 10 + 4;
                copie = rezultat;
            }
             ecran.Text = "" + copie;

        }

        private void cinci_Click(object sender, EventArgs e)
        {

            if (rezultat != 0 && ok == 1)
            {
                nr = nr * 10 + 5;
                copie = nr;
            }
            else
            {
                rezultat = rezultat * 10 + 5;
                copie = rezultat;
            }
            ecran.Text = "" + copie;
        }

        private void sase_Click(object sender, EventArgs e)
        {

            if (rezultat != 0 && ok == 1)
            {
                nr = nr * 10 + 6;
                copie = nr;
            }
            else
            {
                rezultat = rezultat * 10 + 6;
                copie = rezultat;
            }
            ecran.Text = "" + copie;
        }

        private void sapte_Click(object sender, EventArgs e)
        {

            if (rezultat != 0 && ok == 1)
            {
                nr = nr * 10 + 7;
                copie = nr;
            }
            else
            {
                rezultat = rezultat * 10 + 7;
                copie = rezultat;
            }
            ecran.Text = "" + copie;
        }

        private void opt_Click(object sender, EventArgs e)
        {

            if (rezultat != 0 && ok == 1)
            {
                nr = nr * 10 + 8;
                copie = nr;
            }
            else
            {
                rezultat = rezultat * 10 + 8;
                copie = rezultat;
               
            }
            ecran.Text = "" + copie;
        }

        private void noua_Click(object sender, EventArgs e)
        {

            if (rezultat != 0 && ok == 1)
            {
                nr = nr * 10 + 9;
                copie = nr;
            }
            else
            {
                rezultat = rezultat * 10 + 9;
                copie = rezultat;
            }
            ecran.Text = "" + copie;
        }

        private void zero_Click(object sender, EventArgs e)
        {

            if (rezultat != 0 && ok == 1)
            {
                nr = nr * 10;
                copie = nr;
            }
            else
            {
                rezultat = rezultat * 10;
                copie = rezultat;
            }
            ecran.Text = "" + copie;
        }

        private void stergere_Click(object sender, EventArgs e)
        {
            ecran.Text = "";
            a = '#';
            rezultat = 0;
            ok = 0;
            nr = 0;
        }

        private void egal_Click(object sender, EventArgs e)
        { 
            if(a=='*')
            {
                rezultat = rezultat * nr;
            }
            if (a == '-')
            {
                rezultat = rezultat - nr;
            }
            if (a == '+')
            {
                rezultat = rezultat + nr;
            }
            if (a == '/')
            {
                rezultat = rezultat / nr;
            }
            ecran.Text = "" + rezultat;
            ok = 0;
            nr = 0;
            cnt = 0;
        }

        private void radical_Click(object sender, EventArgs e)
        {
            rezultat = Math.Sqrt(rezultat);
            ok = 1;
        }

        private void adunare_Click(object sender, EventArgs e)
        {
            a = '+';
            ok = 1;
            if (cnt != 0)
            {
                if (cnt == 1)
                {
                    rezultat = rezultat * nr;
                }
                if (cnt == 2)
                {
                    rezultat = rezultat + nr;
                }
                if (cnt == 3)
                {
                    rezultat = rezultat / nr;
                }
                if (cnt == 4)
                {
                    rezultat = rezultat - nr;
                }
                ecran.Text = "" + rezultat;
                cnt = 0;
                nr = 0;
            }
            cnt = 2;
            ecran.Text = ecran.Text + " +";
        }

        private void impartire_Click(object sender, EventArgs e)
        {
            a = ':';
            ok = 1;
            if (cnt != 0)
            {
                if (cnt == 1)
                {
                    rezultat = rezultat * nr;
                }
                if (cnt == 2)
                {
                    rezultat = rezultat + nr;
                }
                if (cnt == 3)
                {
                    rezultat = rezultat / nr;
                }
                if (cnt == 4)
                {
                    rezultat = rezultat - nr;
                }
                ecran.Text = "" + rezultat;
                cnt = 0;
                nr = 0;
            }
            cnt = 3;
            ecran.Text = ecran.Text + " :";
        }

        private void scadere_Click(object sender, EventArgs e)
        {
            a = '-';
            ok = 1;
            if (cnt != 0)
            {
                if (cnt == 1)
                {
                    rezultat = rezultat * nr;
                }
                if (cnt == 2)
                {
                    rezultat = rezultat + nr;
                }
                if (cnt == 3)
                {
                    rezultat = rezultat / nr;
                }
                if (cnt == 4)
                {
                    rezultat = rezultat - nr;
                }
                ecran.Text = "" + rezultat;
                cnt = 0;
                nr = 0;
            }
                cnt = 4;
            ecran.Text = ecran.Text + " -";
        }
    }
}
