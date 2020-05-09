koreanbots
==========
A Simple Python API wrapper for KoreanBots.

����
-------------

���� �غ�Ǿ� ���� �ʾƿ� :(

��ġ
-------------

**���̽� 3.6 Ȥ�� �� �̻��� �ʿ��մϴ�.**

.. code:: sh

    python3 -m pip install koreanbots

����
-------------

������ ������Ʈ�ϱ�
~~~~~~~~~~~~~

�ֱ������� ���� ���� ������Ʈ�մϴ�. (discord.py)

.. code:: py

    import discord
    import koreanbots

    client = discord.Client()
    Bot = koreanbots.client(client, 'KoreanBots ��ū')

    @clinet.event
    async def on_ready():
        print(f'{client.user}�� �α����Ͽ����ϴ�.')

    client.run('Discord ��ū')

���̵�� �� ���� ��������
~~~~~~~~~~~~~

discord.py ����

.. code:: py

    import discord
    import koreanbots

    client = discord.Client()
    Bot = koreanbots.client(client, 'KoreanBots ��ū')

    @clinet.event
    async def on_ready():
        print(f'{client.user}�� �α����Ͽ����ϴ�.')

    client.run('Discord ��ū')

discord.py �̻���

.. code:: py

    import koreanbots

    Bot = koreanbots.HTTPClient('KoreanBots ��ū')
    # getBot�� ��ū�� �ʿ����� �ʱ⿡ 'KoreanBots ��ū' �κ��� ���� �����մϴ�.

    Data = loop.run_until_complete(Bot.getBot('653534001742741552'))
    # ��ȯ�Ǵ� �����ʹ� �� ��ũ�� �������ּ���: https://koreanbots.cf/js-sdk/interfaces/_types_.getbyid.html

    print(Data)
