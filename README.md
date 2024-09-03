В каждом отдельно взятом файле реализована проверка через ipytest (Pytest в записных книжках Jupyter). 
ipytest позволяет запускать Pytest в записных книжках Jupyter.

# Установка, выполнив ipytest
pip install ipytest

# Предлагаемый способ импорта выглядит следующим образом:ipytest
import ipytest
ipytest.autoconfig()

# После этого в новой ячейке могут быть выполнены тесты, как в
%%ipytest -qq

def test_example():
    assert [1, 2, 3] == [1, 2, 3]
