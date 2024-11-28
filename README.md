# bedrock-agent-kb-slack

## 事前設定
- AWS認証情報の設定
  - [AWS CLIの設定と認証情報ファイルの設定](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html)
- Bedrock モデルの有効化
  - [Amazon Bedrock 基盤モデルへのアクセスの追加または削除](https://docs.aws.amazon.com/ja_jp/bedrock/latest/userguide/model-access-modify.html)
- ナレッジベースの作成
  - [Amazon Bedrock ナレッジベースを作成する](https://docs.aws.amazon.com/ja_jp/bedrock/latest/userguide/knowledge-base-create.html)
  - [Amazon Bedrock Knowledge Bases とPineconeで低コストなRAGを構築する](https://dev.classmethod.jp/articles/bedrock-kb-rag-pinecone-lowcost/)

## セットアップ手順

1. リポジトリをクローンします。
   ```bash
   git clone https://github.com/sakai-classmethod/bedrock-agent-kb-slack.git
   cd bedrock-agent-kb-slack
   ```
2. `template.yaml`を使用して、AWSリソースをデプロイします。
   ```bash
   rain deploy -r <AWS:Region> template.yaml rag-chatbot-stack
   ```
