当使用jupyter notebook时，使用参数解析器会出现问题，其实只需要在加载参数时加上一点内容即可
``` python
import argparse

parser = argparse.ArgumentParser()
parser.add_argument('--device', default='0,1', type=str, help='设置使用哪些显卡')
parser.add_argument('--no_cuda', action='store_true', help='不适用GPU进行训练')
args = parser.parse_args(args=['--device', '0',  '--no_cuda'])
#args = parser.parse_args(args=[])
print(args)

```
