# Copyright 2016 Jones Magloire (Joxit)
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
FROM node:6-slim

WORKDIR /usr/src/app

ENV WORKDIR=/usr/src/app USER_ID=0

RUN npm install -g carto \
    && npm install -g cartocc \
    && npm install -g js-yaml

COPY bin/* /bin/

ENTRYPOINT ["entrypoint"]

CMD ["cartoyml"]
