�E�{�T���v���R�[�h��docomo Developer support�񋟂̃g�����h�L�����oSDK for Android�iv3.0.1�j�y��OAuth SDK for Android�iv1.1.2�j�𗘗p���Ă���܂��B
�K�X�A�ŐV��SDK�̗L�������m�F���������A�K�v�ɉ����č����ւ��Ă����p���������B
�E�T���v���R�[�h�̓���ɕK�v��API�L�[�Aclient id�Aclient secret�͋L�ڂ���Ă���܂���B
�����g�Ŏ擾���ꂽ���̂������p���������B

�{�T���v���R�[�h�̊e�t�@�C���͉��L�̂悤�ɏ������s���Ă���܂��B
package jp.ne.docomo.smt.dev.webcuration.sample_app
�EPRNGFixes.java�@�FSecureRandom�̐Ǝ㐫�΍�
�ETrendArticleExtractionApplication.java�@�F�g�����h�L�����oSDK�T���v���g���A�v���P�[�V�����N���X Android�A�v���ɂ�����SecureRandom�̐Ǝ㐫�΍�R�[�h�����s����

package jp.ne.docomo.smt.dev.webcuration.sample_app.activity
�EArticleItemViewHolder.java�@�F�L���ꗗ����уL�[���[�h�������ʈꗗ��ListView���ɕ\�����鍀�ڂ�ViewHolder�N���X
�EArticleListFragment.java�F�L���ꗗ��ListView�ŕ\������Fragment MainActivity����ViewPager�̎q�v�f�Ƃ��Đ��������
�EAuthenticationActivity.java�@�F�F�ؐݒ���
�EBaseActivity.java�@�FMainActivity(�L���\�����)�����KeywordSearchActivity(�L�[���[�h�������)�̊��Activity
�EKeywordSearchActivity.java�@�F�L�[���[�h�������
�EMainActivity.java�@�F�L���\�����
�EMessageDialog.java�@�F�^�C�g���A���b�Z�[�W�A�����OK�{�^����\������ėpDialogFragment
�EResultListFragment.java�@�F�L�[���[�h�������ʈꗗ��ListView�ŕ\������Fragment

package jp.ne.docomo.smt.dev.webcuration.sample_app.loader
�EBaseLoader.java�@�F�o�b�N�O���E���h�ň��S�Ƀf�[�^�̎擾���s�����AsyncTaskLoader
�EGenreLoader.java�@�F�o�b�N�O���E���h��SDK����W�����������擾����AsyncTaskLoader
�ESearchLoader.java�@�F�o�b�N�O���E���h��SDK����L�[���[�h�������ʂ��擾����AsyncTaskLoader

package jp.ne.docomo.smt.dev.webcuration.sample_app.oauth
�EAccessTokenManager.java�@�Fdocomo ID OAuth�F�؂ɂ�����A�N�Z�X�g�[�N������эĔF�ؗp���t���b�V���g�[�N���̊Ǘ��N���X
�EEncryptor.java�@�F�����񂨂�уo�C�g�z��̈Í����E���������s���N���X

package jp.ne.docomo.smt.dev.webcuration.sample_app.provider
�ETrendArticleDb.java�@�FTrendArticleProvider�ɂ���ĊǗ������e��e�[�u����`
�ETrendArticleProvide.java�@�F�W���������A�L���R���e���c�f�[�^�A�L���R���e���c��ԁA�{�����O�f�[�^��ێ�����ContentProvider

package jp.ne.docomo.smt.dev.webcuration.sample_app.service
�EArticleStateUpdateService.java�@�F�L���R���e���c��Ԃ�񓯊��ɍX�V����IntentService �{�T���v���A�v���ł͋L���R���e���c�̖��ǁE���Ǐ�Ԃ��X�V����̂�
�EArticleUpdateService.java�@�F�L���R���e���c�f�[�^��񓯊��ɍX�V����IntentService
�ELogDataSendingService.java�@�F�{�����O�f�[�^�̕ۑ���������ѕۑ����ꂽ���O�f�[�^�̈ꊇ���M������񓯊��Ɏ��s����IntentService
