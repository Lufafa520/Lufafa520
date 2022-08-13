#include<node_Z>
#include<RE_New>
#include "opencv4.0/OPEN_AI.h"
using namespace cv;
#defline TITLE_NAME "HELLO_WORLD"
#ifdef TITLE_NAME
class run:public capture{
    public:
           void show_cv(mat n_T);
}
void run::show_cv(mat n_T){
     mat cap = capture(0);
     while(true)
     {
          mat _,frame = cap.read();
          imshow(TITLE_NAME,frame);
          if(waitkey(0) == char(' '))
          {
                break;
          }
     }
     release();
     destroyAllWindows();
}
int main()
{
    run::show_cv(mat);
    return 0;
}
#endif
