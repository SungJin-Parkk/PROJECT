2022년 11월 9일부터 9시부터 6시 까지 

한가람IT교육센터에서 교육을 듣고 있는 박성진 입니다.

지금까지 배웠던 교육과정 및 프로젝트들을 나열하겠습니다.


# C#의 개념 및 구문 

string은 문자 int는 숫자라는 아주 기초적인 것도 몰랐지만

열심히 강의를 들어서 밑에 구문은 작성 할만한 실력과 개념이 되었습니다.

처음부터 끝까지 짠 코딩이며 교육센터의 시험중 하나였습니다.

![ㅇㅇ](https://github.com/SungJin-Parkk/Project/blob/main/img/%EC%B2%AB%EB%B2%88%EC%A7%B8.png)

## 코딩
```
using System; 
using System.Collections.Generic;
using System.Windows.Forms;

namespace MyFirstCSharp
{
    public partial class Chap24_Algorithm_Exam01 : Form
    {
        public Chap24_Algorithm_Exam01()
        {
            InitializeComponent();
        }

        private void btnMakeRandomAndSum_Click(object sender, EventArgs e)
        {
            txtResult.Text = "";
            // 랜덤 난수 생성 및 없는 수 합치기.
            Random ran = new Random();
            
            for (int z = 0; z < 20; z++)
            {
                int iValue = ran.Next(0, 20);
                txtResult.Text += iValue.ToString() + ",";
            }

            string[] T1 = txtResult.Text.Split(',');
            int[] zip2 = new int[T1.Length];
            for (int s = 0; s < T1.Length - 1; s++)
            {
                zip2[s] = Convert.ToInt32(T1[s]);
            }
            

            int[] zip = new int[21];

            for (int i = 0; i < 21; i++)
            {
                zip[i] = i;
            }
            int[] zip3 = new int[] { };
            for (int d = 0; d < 19; d++)
            {
                for (int s = 0; s < 19; s++)
                {
                    if (zip[d] == zip2[s])
                    {
                        zip[d] = 0;
                        
                    }
                }
            }
            int b1 = 0;
            for(int nn=0; nn<20; nn++)
            {
                 b1 += zip[nn];
            }
            MessageBox.Show($"{b1}");
        }
    }
}

```

# 미니 프로젝트

3명을 조를 이루어 

![ㅇㅇ](https://user-images.githubusercontent.com/118166199/215767288-3a4110d5-43d4-42b3-8d3a-ae86746b4a81.png)
