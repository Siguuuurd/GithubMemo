#Chef�̃C���X�g�[���Ɛݒ�

�Q�l�T�C�g�F[http://note.miyabis.jp/2013/12/chef-%E3%82%92-windows-%E3%81%A7%E4%BD%BF%E3%81%A3%E3%81%A6%E3%81%BF%E3%82%8B.html]

#Chef�̃C���X�g�[��
1. 
http://www.opscode.com/chef/install/#options
�܂���
http://opscode.com/chef/install.msi

�R�}���h�v�����v�g�ŉ��L�����s����ƃo�[�W�������\�������B
chef-solo -v


1. Windows ���p�� Cookbook �擾
�ȉ��̂Q���擾����B
http://community.opscode.com/cookbooks/windows
http://community.opscode.com/cookbooks/chef_handler


1. chef-solo �̐ݒ�
C:?chef?solo.rb

```�ȉ�����͂���
cookbook_path ["C:?chef?repo?cookbooks"]
```

1. chef�ň��k�t�@�C�����𓀂Ƃ�����Ƃ��ɃR�}���h�Ŏ��s�ł���𓀃c�[��(7-zip)[Inx-7-zip]
[Inx-7-zip]: https://supermarket.chef.io/cookbooks/seven_zip "chef�ň��k�t�@�C�����𓀂Ƃ�����Ƃ��ɃR�}���h�Ŏ��s�ł���𓀃c�[��(7-zip)"

```�ȉ�����͂���
C:?chef?repo �t�H���_�ɉ��L�̓��e�� 7-zip.json �t�@�C�����쐬����B
{
	"run_list": ["recipe[7-zip]"]
}
```