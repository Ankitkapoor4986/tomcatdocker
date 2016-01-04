FROM wnameless/oracle-xe-11g
ADD scripts data/scripts
RUN  chmod +x data/scripts/prepare-db.sh && /usr/sbin/startup.sh & sleep 40 && export ORACLE_HOME=/u01/app/oracle/product/11.2.0/xe && export PATH=$ORACLE_HOME/bin:$PATH && export ORACLE_SID=XE && /data/scripts/prepare-db.sh
