# NDT7 Speed Test

[English](README.md) | 日本語

Measurement LabのNDT7基盤を使い、iOS・Androidでダウンロード速度とアップロード速度を測定するFlutterアプリです。独自の測定サーバーを用意する必要はありません。

## 主な機能

- 初回測定前の同意画面
- ダウンロード・アップロードの手動速度測定
- 各測定フェーズの進捗表示
- 端末内に保存する測定履歴とWi-Fi・モバイル回線フィルター
- 結果の詳細表示とテキスト共有
- 設定画面からの同意撤回

測定にはMeasurement Labのサービスを利用するため、送信される測定データは同サービスのデータ取扱いに従います。アプリが保存する履歴は、ユーザーが共有しない限り端末内に保持されます。

## ビルド

```bash
flutter pub get
flutter analyze
flutter test
flutter build apk --debug
```

GitHub ActionsではAndroidのデバッグAPKと未署名のiOS成果物を生成できます。未署名のiOS成果物は、通常のApp Store配布物や端末へそのままインストールできるリリースではありません。

## ライセンス

独自コードはプロプライエタリで、すべての権利を留保します。詳細は [LICENSE](LICENSE) を参照してください。直接依存する第三者コンポーネントのライセンス原文は [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) に保存し、アプリのアセットにも含めています。
